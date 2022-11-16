# D END

## Introdução
A empresa Dom Rock propôs um desafio acadêmico para os alunos do 6º semestre do curso de Banco de Dados da FATEC-SJC, a fim de estimular o desenvolvimento das matérias do período, os preparando para o mercado de trabalho.

## Proposta 
O objetivo da parceria era o desenvolvimento de uma API que realizasse a análise dos dados de duas bases, sendo seus clientes PF e operadora de convênio de saúde; para conciliar os registros e identificar débitos técnicos entre as contas, alem de auxiliar na criação de um plano de ação para evitar futuras inconsistências.

## Tecnologias utilizadas
- Python: linguagem de programação definida por ser melhor em análise de dados. Utilizada na conexão com o banco, manipulação de planilhas e criação de arquivos logs. 
- MongoDB: banco de dados não relacional, orientado a documentos. Utilizado para o armazenamento de dados vindos de arquivos ".csv". Banco utilizado com a Aggregation Framework para desenvolver a lógica que identifica inconsistências nos dados providos entre cliente e empresa.
- SQL Server: sistema gerenciador de Banco de dados relacional, onde foram realizados os scripts SQL para prototipação das colunas e tabelas que provem o Data Warehouse.
- Power BI:serviço de análise de negócios e análise de dados. Utilizado durante o projeto para o consumo do Data Warehouse, gerando gráficos e métricas das análises realizadas.
- Microsoft Azure: serviço de computação em nuvem operado para deploy do Data Warehouse.
- Jira: ferramenta utilizada para a criação, acompanhamento e priorização de tarefas.

## Contribuições individuais 

Neste projeto atuei especificamente no backend. De início conectei a API  com o banco, e logo depois li o arquivo ".cvs", manipulei o tipo dos dados e os inseri no MongoDB. 

<details>
  <summary>Click aqui pra visualizar</summary>
  
  ```js
  @staticmethod
    def create_connection_db():
        load_dotenv()
        try:
            logger.info('Opening database connection')
            url_mongodb = os.environ['BANCO_CREDENTIALS']
            logging.info('Establishing connection')
            cluster = MongoClient(url_mongodb)

            db = cluster[os.environ['CLUSTER']]
            logging.info('Get a cluster')
            return db

        except Exception as e:
            logger.error('Connection error, bad credentials ')
            return Exception

    @staticmethod
    def get_collection_db(bool: bool):
        try:
            logger.info('Create a connection')
            collection = Database_configs.create_connection_db()

            logger.info('Get a collection name')
            if bool:
                return collection[os.environ['COLLECTION']]
            return collection[os.environ['COLLECTION_LOGS']]
        except Exception as e:
            logger.error('error while get a collection name')
  ```
</details>

Feito isso, precisei criar um arquivo ".log" para armazenar os logs sobre o que estava acontecendo com a API.

<details>
  <summary>Click aqui pra visualizar</summary>
  
  ```js
      @staticmethod
    def read_csv():
        logger.info('read a csv')
        try:
            url_csv = ""

            data = pd.read_csv(url_csv, sep=',',
                            low_memory=False)
            idFile = data['_id']
            for id in idFile:
                logger.info('Get a file id: ' + str(id))
            return Csv_service.transform_fields(data)
        except FileNotFoundError as error:
            logger.info('Error file not found')
            return error
        except ValueError as error:
            logger.error('Parser error during convertion')
            return error

    @staticmethod
    def transform_fields(data):
        columns = pd.DataFrame(data)
        transform_columns_data = []
        transform_columns_value = []
        for col in columns:
            if 'dt_' in col:
                transform_columns_data.append(col)
        for item in transform_columns_data:
            data[item] = pd.to_datetime(data[item])

        for col in columns:
            if 'valor' in col: 
                transform_columns_value.append(col)
        for item in transform_columns_value:
            data[item] = data[item].astype('double')
        return data
  ```
</details>

## Aprendizados efetivos

### Hard Skills

- Manipulação de planilhas com a framework Pandas;
- Conexão entre back-end Python e banco de dados MongoDB;
- Criação de aquivos logs com o auxílio da linguagem Python.

### Soft Skills

- Gestão de tempo para realizar as tasks definidas; 
- Trabalho em equipe.
