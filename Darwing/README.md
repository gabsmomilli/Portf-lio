# Web Bot - HeySeries

## - Descrição do projeto:

O Projeto Integrador Darwing visa estimular o desenvolvimento dos alunos do 2° semestre de Banco de Dados da FATEC de São José dos Campos. Um cliente escolhido pela Fatec, desafiou os alunos do 2° semestre com a proposta de desenvolver um sistema gerenciador de tarefas. 

A proposta do projeto é a de que um grupo de alunos desenvolva uma aplicação administrativa de afazeres, sendo para uma unica pessoa ou até mesmo para uma empresa. O padrão de projeto proposto é MVC em Java utilizando a framewok Spring Boot, oferecendo mais agilidade para o processo de desenvolvimento, dado que os desenvolvedores conseguem reduzir o tempo gasto com as configurações iniciais.

Com o inicio a pandemia, a FATEC deve de se adequar aos métodos de ensino remoto, atrazando o periodo de ensino e de desenvolvimento das aulas e projeto. Sendo assim, com tempo reduzido, as sprints tiveram apenas duas semanas para cada entrega.

Darwing foi o nome definido pelo grupo, dadndo referencia ao Charles Darwin.

Foi decidido o uso do banco de dados MySQL por conveniente estudo do mesmo durante o periodo. De inicio o grupo realizou o que seria o rascunho do banco de dados, no qual foi remanejado mais tres vezes durante todo o processo. Chegando no seguinte final: 

### COLOCAR FOTO DO DESENHO DO BANCO 

No desenvolver do projeto, foi validado com o cliente o que seria o MÍNIMO PRODUTO VIÁVEL, sendo determinado como um banco de dados enxuto de dados, sendo um pouco mais descritivo em cada tarefa e back-end seguindo a filosofia de desenvolvimento de software que consiste em aplicar técnicas simples que facilitam a escrita e a leitura de um código.

Para o desenvolvimento da aplicação o grupo se subdividiu para organizar as tarefas. Banco de dados e back-end.

- BACK-END: 
    - MODELS : procuraram cursos gratuitos/ baratos que ensinassem como iniciar um projeto Java utilizando Spring Boot. O grupo deve grande dificuldade em iniciar as models sendo que desenho do banco de dados teria sido remanejado diversas vezes, já que a model é exatamente o modelo da tabela em si que esta no banco de dados, como os tipos de dados armazenados em cada coluna e seus relacionamentos.
    - BANCO DE DADOS : para a integração com o banco de dados, foi definido no POM as dependencias do banco de dados e as definições como nome do banco, porta e senha no APPLICATION. A dificuldade nesata atividade foi entender onde cada informação iria ser determinada, qual arquivo e ordem.
    - REPOSITORY: ele ministra a ligação a determinada classe do Model com possibilidade de persistir no banco de dados. Lá são definidas as Querys, porém em outro padrão com que os alunos estavão acostumados em desenvolver, pois caso o banco de dados mudasse para Oracle, por exemplo, não teria de ser reformulado muitas linhas de codigo além do POM com as dependedncias do novo banco e no APPLICATION com as definições de conexão.
    -  SERVICE : todos os serviços onde estão as regras de negócio, validações e o que mais for preciso. No caso do Darwing, nesta camada que foi criada as validações, como:
        - se haviam campos nulos;
        - se o desenvolvedor já não estava cadastrado;
        - carga horaria maior que 0 horas. 
     entre outras que foram requisitadas neste projeto.
    - CONTROLLER : classe responsável pela preparação de um modelo de Map com dados a serem exibidos pela view e pela escolha da view correta. Basicamente ele é o responsável por controlar as requisições indicando quem deve receber as requisições para quem deve responde-las. Entregando então pra determinada barra (/tarefa) o que é requisitado como metodo de requisição HTTP.
    
- BANCO DE DADOS 
    - MYSQL : devido o inicio a materia de Arquitetura e Modelagem e Banco de Dados, visando a utilização do banco de dados MySQL, o grupo determinou que este seria o ideal, já que poderiam tirar dúvidas com o professor que dava a tal materia.
 - 

Por fim o projeto teve algumas dificuldades, perca de alguns colegas desistentes do curso, porém, em geral, o grupo foi o melhor e único a tirar 10!

## - Tecnologias 
Foi introduzido a linguagem Python para os alunos do 1° semestre, logo projeto deveria seguir com o desenvolvimento com a mesma. Como o a equipe distinguia de conhecimentos sobre desenvolvimento e nomenclaturas como "raspagem de dados", logo a dificuldade na comunicação entre eles e com os professores se manifestou. Por fim realizaram a raspagem de dados com sucesso, utilizando um pacote chamado Beautiful Soup, porém sem armazená-los em algum local. Devido a baixa granularidade dos dados, foi definido o uso de um banco de dados não relacional, armazenariam o nome da série, gênero, data de lançamento e nota em formato de Json; sendo ele o CouchDB. Para fazer a conexão entre os dados e a interface gráfica, foi empregada a framework Flask. E por fim, o front-end foi desenvolvido utilizando HTML, CSS e Javascript para interface e a manipulação dos dados, ato seria a filtragem dos dados mostrados.

- Python:
  Linguagem de programação, desenvolvida para ser simples, fácil de aprender e versátil, logo, para ser utilizá-la em diversas atividades. Sendo ótima para ser a 1° linguagem de se aprender, também é uma das mais utilizadas no mundo e valorizada por poder ser utilizada em diversas áreas, pode se diferenciar de outras linguagens.
  
 - Beautiful Soup: 
    Pacote Python para análise de documentos HTML e XML. Ele cria uma árvore de análise para páginas analisadas que podem ser usadas para extrair dados de HTML, o que é útil para web scraping.
  
- Flask:
  Micro framework multiplataforma escrito em Python para gerenciamento no mesmo e disponível em código aberto, oferece um modelo simples para desenvolvimento web. Neste caso lançando as informações do banco de dados até o front-end.
  
- CouchDB:
  Banco de dados NoSQL orientado a documentos. Utiliza JSON como formato de dados e JavaScript como linguagem de consulta. Diferente da maioria dos outros bancos de dados, seu conteúdo é acessado e modificado através de uma API REST.

- Javacript:
  Linguagem de programação que permite a criação de conteúdos que se atualizam dinamicamente, controla multimídias, imagens animadas, pesquisas por filtros, entre outros.

## Contribuições individuais

Para desenvolver o back-end do projeto, foi decidido a aproveitamento da linguagem Python e o uso das bibliotecas compatíveis com a mesma. Literalmente foi pesquisado por "raspagem de dados" no Google e vários vídeos e passo-a-passo apontados. O pacote Beautiful Soup era o mais citado dentre os links, logo foi decidido a implementado. 

Deve ser importado no inicio da classe, conforme a figura a baixo:

![image](https://user-images.githubusercontent.com/55815856/142081595-0be8f770-2b7b-42d1-9b62-60a945e39e26.png)

Declarar o site que deseja consumir:

https://www.imdb.com/search/title/?title_type=tv_series&release_date=1980-01-01,2019-12-31&user_rating=,%27%2710.0&count=250

![gfhadgfadgaidaygafgoaehgouaehg](https://user-images.githubusercontent.com/55815856/141889016-3b3472d9-ccda-4ad0-ba75-1c31019e81ac.PNG)

Selecionando dados relevantes para API consumir:

- Coleta de dados específicos:

    - Visualização através do browser: 
    
    Botão direito do mouse -> Inspecionar -> Elementos
    
    ![image](https://user-images.githubusercontent.com/55815856/141889579-7efcc2a8-58ef-470e-9838-3af923fbce9c.png)
 
    - Como os dados são "capturados" pelo pacote Beautiful Soup:
    
    Utilizando a visualização fornecida pelo browser, pode-se ver o caminho para submeter tal dado.
    
    ![puxando dados necessarios](https://user-images.githubusercontent.com/55815856/141889757-f9f27295-51e1-454f-a92d-f112f4c435f9.PNG)

Foram encontradas dificuldades em paginar devido a diferença entre URL e quantidade apresentada; raspar outros sites também foi um impedimento pois não foi apresentado métodos ágeis de realizar tal processo. Por fim foi decidido manter um único site com uma única pagina sendo consumida.

Após extrair os dados, resolvido que os dados deveriam ter as seguintes modificações:

    - O caractere apóstrofo deveria ser retirado dos títulos;
   
    - As notas deveriam ser números quebrados;
    
    - Alguns gêneros tinham erro de escrita com "/n", então deveriam ser retirados;
    
    - Caracteres como números romanos, parêntese aperto e fechado, sinal meia-risca deveria ser retirados das datas de lançamento;
    
    - Deveriam ser mantidos somente o ano de lançamento, ignorando o ano em que a serie encerou.
        Exemplo: (2007-2012) -> 2007

Foram estudadas as possibilidades de local e como efetuar o armazenamento os dados raspados, até que fosse concluída como melhor ideia a utilização de um banco de dados não relacional, pois não havia uma massa de granularidade dentre os dados. O CouchDB foi indicado por alunos mais experientes da mesma faculdade. Para dispor do banco de dados, é necessário declarar o login e senha código em Python para autenticação.

- Como autenticar no CouchDB:

![login couchdb](https://user-images.githubusercontent.com/55815856/141023643-b801c2e9-99aa-4a64-a266-1d41c992f9ba.PNG)


- Json no banco de dados:

![image](https://user-images.githubusercontent.com/55815856/142066587-4ac894e6-36b3-446b-9e38-7b083705c0bc.png)


## Aprendizados efetivos
- SCRUM: com o desenvolver deste projeto é possível informar-se de como funciona o scrum. O papel de cada indivíduo da equipe e como a comunicação pode ser falha. Cada etapa ou avanço deve ser inspecionado, de modo a identificar se são necessárias possíveis mudanças ou adaptações. Se no sprint anterior forem identificadas necessidades de mudanças é crucial que a equipe Scrum esteja preparado e capacitado para realiza-las. Realizar reuniões para manter a comunicação entre os indivíduos e reportar os andamentos das tasks, dificuldades e ou ideias.

- METODOLOGIA ÁGIL: sistema organizacional que contribui para o desenvolvimento de soluções mais eficientes e dinâmicas em grupo, buscando otimizar fluxos de trabalho, melhorar a produtividade de projetos e elevar as perspectivas de sucesso do seu negócio. Aperfeiçoando a produtividade de projetos e aumentar as perspectivas dos resultados. Mantendo como prioridade a satisfação do cliente por meio de entregas de valor contínuas e rápidas. Garantindo a colaboração das partes envolvidas em todo o projeto, por meio de reuniões continuas.

- PYTHON: Devido a simplicidade da linguagem e a demanda de menos código para concluir tarefas básicas quando comparadas a padrões de outras linguagens, sintaxe intuitiva, documentação e passo-a-passo aos montes, bibliotecas gratuitas e por ser uma linguagem interpretada, Python não causa grandes dificuldades em ser utilizada mesmo por desenvolvedores iniciantes. Há muitos cursos bons e gratuitos recheados de conteúdo, basta praticar.

- RASPAGEM DE DADOS: O termo "raspagem de dados" por ser muito técnico, aparenta ser um exercício complexo, o que pode ser para indivíduos iniciantes á programação. Ao           realizar a elaboração do mesmo, muitos relatam ser um experimento interessante e divertido, principalmente quando administrado com a famosa biblioteca Beautiful Soup e disposta com vários vídeos de como utilizá-la. Pode ser relatado dificuldades na utilização caso o desenvolvedor desconheça HTML.
    
- MANIPULAÇÃO DE DADOS: Para realizar a manipulação de dados em Python, basta seguir a documentação do mesmo, contudo, muitos desenvolvedores iniciantes optam por                vídeos. um canal bem famoso por trilhas em Python é o canal Curso em Vídeo do professor Gustavo Guanabara. O curso é extenso, entretanto completo e recheado de                   atividades para o aluno treinar.

- TRANSFORMAR OS DADOS EM JSON: o conceito de criar um modelo (model do projeto) aparenta ser abstrato, o que realmente é, porém é o que estrutura ao dado. Como foi              utilizado banco de dados não relacional, o Json foi simples.
