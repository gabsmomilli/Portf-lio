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

## Contribuições pessoais para o projeto
Neste projeto atuei especificamente no backend. De início conectei a API  com o banco, e logo depois li o arquivo ".cvs", manipulei o tipo dos dados e os inseri no MongoDB. 

![image](https://user-images.githubusercontent.com/55815856/201440608-966ce205-6329-49f2-9296-0ceb7c682e6c.png)

Feito isso, precisei criar um arquivo ".log" para armazenar os logs sobre o que estava acontecendo com a API.

![logs](https://user-images.githubusercontent.com/55815856/201440366-99c54f03-bb9b-4b96-a5e3-f31cc3939389.PNG)

## Conhecimentos adquiridos
### Soft Skills
- Gestão de tempo para realizar as tasks definidas; 

### Hard Skills
- Manipulação de planilhas com a framework Pandas;
- Conexão entre back-end Python e banco de dados MongoDB;
- Criação de aquivos logs com o auxílio da linguagem Python;
