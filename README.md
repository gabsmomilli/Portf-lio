# Web Bot - HeySeries

## - Descrição do projeto:

O Projeto Integrador HeySeries visa estimular o desenvolvimento dos alunos do 1° semestre de Banco de Dados da FATEC de São José dos Campos. A proposta do projeto é desenvolver um desafio onde os professores deram a solução para que os grupos determinassem o problema. 

A proposta do projeto é a de que um grupo de alunos desenvolva uma aplicação web bot, utilizando o problema proposto pelo próprio grupo. A técnica proposta é "raspagem de dados", dado como um processo de operar uma aplicação para extrair dados valiosos de uma fonte, para utilizá-los a seu favor. Raspagem de conteúdos pode ser então "replicada" ou manipulada conforme o necessário.

Um prazo para entrega foi estipulado e chamado de "sprint", logo introduzido a metodologia ágil e o scrum. “Masters” foram designados para cada grupos, e os mesmos seriam alunos mais experientes do ultimo semestre do curso de banco de dados, seus objetivos eram de gerenciar e solucionar impedimentos que o grupo enfrentasse. Foi determinado o uso do gitlab durante cada sprint.

Pensamos em resolver o seguinte problema: indicação de séries com boas notas de avaliação pelo público.

Logo escolhemos o nome HeySeries, fazendo referência inteligencia artificial da Apple "Siri".

A ideia foi a de desenvolver uma aplicação web bot que faria raspagem de dados em um site, coletando dados referentes a seriados, seus respectivos gêneros, ano de lançamento e nota, sendo armazenados em um banco de dados, onde os mesmos serão disponibilizados para o front-end otimizar a experiência do usuário ao buscar por séries com melhores notas.

No desenvolver do projeto, foi validado com o cliente o que seria o MÍNIMO PRODUTO VIÁVEL, sendo determinado como uma raspagem simples de um único site de séries, junto de seus respectivos dados. Mostrando apenas as 10 melhores series com maiores notas.

Para o desenvolvimento da aplicação o grupo se subdividiu para organizar as tarefas. Inicialmente seria um equipe back-end e outro front-end.
- BACK: 
    - RASPAGEM DE DADOS: procuraram cursos gratuitos que ensinassem como raspar dados de um site utilizando Python. A organização deste time foi confusa, já que os dois membros basicamente procuraram as respostas separadamente, assim tomando o dobro de tempo por falta de comunicação. Por fim, um destes alunos conseguiu exito na tarefa e trazendo alguns dados como "teste". Um ajudou o outro após aprender como funcionava tal processo.
    - MANIPULAÇÃO DOS DADOS: alguns destes dados vieram de forma distinta, então a manipulação foi necessária. A atividade foi constituída na retirada de alguns caracteres especiais no nome do filme, gênero e data.
    - INSERÇÃO NO BANCO DE DADOS: este tópico exigiu um foque maior, pois os membros do grupo não sabiam como os bancos funcionavam e como escolher um que fosse adequado para armazenar dados de um determinado tipo. Com ajuda de nossos masters e outros colegas mais experientes, foi decidido pelo grupo que o ideal seria um banco de dados não relacional, pois seria armazenado em formato de Json e não em tabelas e colunas como no relacional.
    - MANDAR DADOS DO BANCO PARA O  FRONT: neste ponto nosso front já estava funcionando, mas ainda não consumia dados do banco, eram dados locais no próprio HTML. Novamente alguns colegas mais experientes nos deram algumas ideias de quais frameworks podíamos utilizar. Foi decidido utilizar a micro-framework Flask devido o acesso que um dos alunos tinham em uma plataforma de cursos voltados para área da tecnologia.
 - FRONT:
    - HTML e CSS: os alunos designados para a execução do front-end, começaram a desenvolver a interface gráfica com HTML e CSS, e logo tiveram grandes resultados de como ficaria o projeto em vista do usuário. A área de interação era simples, com uma logo desenvolvida no Canvas e transformada em PNG, uma breve descrição sobre o projeto e, porque foi desenvolvido, e a listagem das 10 series no próprio HTML.
    - PUXAR DADOS DO BANCO: além da framework que o grupo de back decidiu utilizar, a equipe de front precisaria de JavaScript para manipular os dados como o manuseio de filtros e busca. Este foi um dos processos mais demorados e trabalhosos da equipe, em vista o grau de dificuldade.

Por fim o projeto teve algumas dificuldades, perca de alguns colegas desistentes do curso, porém, em geral, o grupo foi o melhor e único a tirar 10!


### - Cliente

CEETEPS - Centro Estadual de Educação Tecnológica Paula Souza
O Centro Paula Souza administra as Faculdades de Tecnologia (Fatecs) e Escolas Técnicas Estaduais (Etecs) nas cidades do Estado de São Paulo. As Etec atendem mais de 100 mil estudantes nos níveis de ensino Médio e Técnico, para os setores Industrial, Agropecuário e de Serviços, em 78 habilitações. Nas Fatecs, mais de 20 mil alunos estão distribuídos em vários cursos Superiores de Graduação.

Faculdade de Tecnologia de São José dos Campos.
A Faculdade de Tecnologia de São José dos Campos foi criada no dia 2 de março de 2006 conforme o Decreto Nº 50.580 publicado no Diário Oficial: A Fatec é uma Faculdade Pública Estadual e todos os cursos oferecidos são gratuitos.

O Curso de Tecnologia
De uma forma geral a formação do Tecnólogo, além de aspectos técnicos, envolve também, uma base de caráter social, ético, filosófico e ambiental que faz deste cidadão um profissional ciente de sua inserção e responsabilidades no meio social que integra. Esta bagagem técnica e sócio-ambiental adquirida implicará em um tecnólogo que realiza suas atribuições seguindo sempre normas de segurança, higiene e proteção ao meio-ambiente. Inclui, também, aspectos de empreendedorismo que possibilita sua dedicação a direção e gerenciamento do seu próprio negócio, prestação de serviços de assessoria, ao ensino e a pesquisa tecnológica dentro de seu campo profissional.

### - Features
- Raspagem dos dados
- Armazenar os dados coletados 
- Visualização gráfica de informações
- Filtros para melhor aplicação dos dados

### - Requisitos
#### Funcionais

| Requisitos Funcionais                                                  | Código | Prioridade | Sprint |
|------------------------------------------------------------------------|--------|------------|--------|
|Desenvolver um programa em linguagem Python que faça a coleta de dados em um site que disponibilize as informações necessárias             | RF01   | 1          | 1      |
| Reunir os valores coletados em um banco de dados | RF02   | 1          | 2      |
| Interface agradavel para o usuario com as 10 melhores series                                | RF03   | 1          | 2      |
| Meios de filtragem para que o usuario consiga escolher um determinado ano de lançamento, genero ou nota                                                 | RF04  | 1          | 3     |



#### Não funcionais

| Requisitos Não Funcionais                            | Código | 
|------------------------------------------------------|--------|
| Seguir os conceitos da metodologia ágil	         | RNF01  |
| Scrum                  | RNF02  |

### - Tecnologias 
Foi introduzido a linguagem Python e nosso meio academico, logo o grupo entrou em consenço para utilizá-la. Como todo o grupo Vitoriosos destinguia de conhecimentos sobre desenvolvimento e nomenclaturas como "raspagem de dados", ocorreu um pouco de dificuldade na comunicação com os professores. Por fim realizamos a raspagem de dados com sucesso, porém precisavamos armazená-los em algum lugar, no caso um banco de dados. Devido a baixa granularidade dos dados, resolvemos optar por um banco de dados não relacional, onde uma unica tabela armazenaria o nome da serie, genero, data de lançamento e nota; sendo ele o CouchDB. Para fazer esta "ponte" entre os dados e a interface grafica, foi utilizada a framework Flask. E por sim, nosso frontend foi desenvolvido utilizando HTML, CSS e Javascript para interface e a manipulação dos dados, que no caso seria a filtragem dos dados mostardos.

- Python:
  Linguagem de programação, desenvolvida para ser simples, fácil de aprender e versátil, logo, para ser utilizá-la em diversas atividades. Sendo ótima para ser a 1° linguagem de se aprender, também é uma das mais utilizadas no mundo e valorizada por poder ser  utilizada em diversas áreas, pode se diferenciar de outras linguagens.
  
- Flask:
  Micro-framework multiplataforma escrito em Python para gerenciamento no mesmo e disponível em código aberto, oferece um modelo simples para desenvolvimento web. Neste caso lançando as informações do banco de dados até o front-end.
  
- CouchDB
  Banco de dados NoSQL orientado a documentos. Utiliza JSON como formato de dados e JavaScript como linguagem de consulta. Diferente da maioria  dos outros bancos de dados, seu conteúdo é acessado e modificado através de uma API REST.

- Javacript
  Linguagem de programação que permite a criação de conteúdos que se atualizam dinamicamente,  controla multimídias, imagens animadas, pesquisas por filtros, entre outros.

### Contribuições individuais 
A primeira parte do projeto foi coletar os dados de um site que daria notas as series, junto a algumas outras informações importantes para o grupo. O grupo Vitiriosos não fazia ideia de como realizar este processo, logo nos divimos em 2 grupos, sendo eles: front e back. Eu e mais um rapaz ficamos buscando na meios de como coletar dados de outro site individualmente, pois a ideia original era coletar dados de 3 sites a fim de tirar uma media da nota entre eles.
Por fim eu fui a primeira a conseguir raspar os dados do site OMELETE (https://www.imdb.com/search/title/?title_type=tv_series&release_date=1980-01-01,2019-12-31&user_rating=,'
    '10.0&count=250), porém encontramos dificuldades em paginar, já que seriam muitas paginas este processo, entretanto entramos em consenço com nossos professores de que não teria grandes problemas, a demais, não conseguimos raspar dados de outros sites devido a grande diferença entre todos eles. Por fim decidimos manter um unico site com uma unica pagina sendo raspada de fato. Esta parte foi desenvolvida por mim, assim como a injeção dos mesmos em um banco de dados.
    Novamente como um grupo nos estudamos as posssibilidades de onde e como armazenar os dados raspados, chegamos a conclusão de que a melhor ideia seria um banco de daos não relacional, pois não quebrariamos em tantos pedaços estes dados. O CouchDB nos foi indicado por alunos mais experientes da mesma faculdade. Não tive grandes dificuldades em utilizar o banco de dados, só precisaria ter o login e senha declarados no codigo em Python, e astabela e as respectivas colunas que guardariam os dados coletados.

- Puxando site Omelete:

![gfhadgfadgaidaygafgoaehgouaehg](https://user-images.githubusercontent.com/55815856/141889016-3b3472d9-ccda-4ad0-ba75-1c31019e81ac.PNG)

- Coleta de dados expecificos:

![image](https://user-images.githubusercontent.com/55815856/141889579-7efcc2a8-58ef-470e-9838-3af923fbce9c.png)

![puxando dados necessarios](https://user-images.githubusercontent.com/55815856/141889757-f9f27295-51e1-454f-a92d-f112f4c435f9.PNG)

- Armazenamento no banco de dados:


- Como logar no CouchDB:

![login couchdb](https://user-images.githubusercontent.com/55815856/141023643-b801c2e9-99aa-4a64-a266-1d41c992f9ba.PNG)


### Aprendizados efetivos



