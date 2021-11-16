# Portifólio

## Web Bot - HeySeries

### - Descrição do projeto:
Desenvolver um web bot que faça uma raspagem de dados em um site, coletando dados referentes a seriados, seus respectivos generos, ano de lançamento e nota, sendo armazenas em um banco de dados, onde as mesmas serão disponibilizadas para o frontend consumir e otimizar a experiência do usuário em indicação de séries.

### - Proposta comercial:
O objetivo do projeto é que um grupo de alunos desenvolva uma aplicação em que seja um webbot, usando o na solução de um problema proposto pelo proprio grupo.

### - Cliente

CEETEPS - Centro Estadual de Educação Tecnológica Paula Souza
O Centro Paula Souza administra as Faculdades de Tecnologia (Fatecs) e Escolas Técnicas Estaduais (Etecs) nas cidades do Estado de São Paulo. As Etec atendem mais de 100 mil estudantes nos níveis de ensino Médio e Técnico, para os setores Industrial, Agropecuário e de Serviços, em 78 habilitações. Nas Fatecs, mais de 20 mil alunos estão distribuídos em vários cursos Superiores de Graduação.

Faculdade de Tecnologia de São José dos Campos.
A Faculdade de Tecnologia de São José dos Campos foi criada no dia 2 de março de 2006 conforme o Decreto Nº 50.580 publicado no Diário Oficial: A Fatec é uma Faculdade Pública Estadual e todos os cursos oferecidos são gratuitos.

O Curso de Tecnologia
De uma forma geral a formação do Tecnólogo, além de aspectos técnicos, envolve também, uma base de caráter social, ético, filosófico e ambiental que faz deste cidadão um profissional ciente de sua inserção e responsabilidades no meio social que integra. Esta bagagem técnica e sócio-ambiental adquirida implicará em um tecnólogo que realiza suas atribuições seguindo sempre normas de segurança, higiene e proteção ao meio-ambiente. Inclui, também, aspectos de empreendedorismo que possibilita sua dedicação a direção e gerenciamento do seu próprio negócio, prestação de serviços de assessoria, ao ensino e a pesquisa tecnológica dentro de seu campo profissional.

### - Features
Raspagem dos dados
Armazenar os dados coletados 
Visualização gráfica de informações
Filtros para melhor aplicação dos dados

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


- Coleta de dados
- Armazenamento no banco de dados
- Como logar no CouchDB:

![login couchdb](https://user-images.githubusercontent.com/55815856/141023643-b801c2e9-99aa-4a64-a266-1d41c992f9ba.PNG)


### Aprendizados efetivos



