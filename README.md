# Web Bot - HeySeries

## - Descrição do projeto:

O Projeto Integrador HeySeries visa estimular o desenvolvimento dos alunos do 1° semestre de Banco de Dados da FATEC de São José dos Campos. A proposta do projeto é desenvolver um desafio onde os professores deram a solução para que os grupos determinassem o problema. 

A proposta do projeto é a de que um grupo de alunos desenvolva uma aplicação web bot, utilizando o problema proposto pelo próprio grupo. A técnica proposta é "raspagem de dados", dado como um processo de operar uma aplicação para extrair dados valiosos de uma fonte, para utilizá-los a seu favor. Raspagem de conteúdos pode ser então "replicada" ou manipulada conforme o necessário.

Um prazo para entrega foi estipulado e chamado de "sprint", logo introduzido a metodologia ágil e o scrum. “Masters” foram designados para cada grupos, e os mesmos seriam alunos mais experientes do ultimo semestre do curso de banco de dados, seus objetivos eram de gerenciar e solucionar impedimentos que o grupo enfrentasse. Foi determinado o uso do gitlab durante cada sprint.

Ideia do grupo: indicação de séries com boas notas de avaliação pelo público.

Logo escolheram o nome HeySeries, fazendo referência inteligencia artificial da Apple "Siri".

A ideia foi a de desenvolver uma aplicação web bot que faria raspagem de dados em um site, coletando dados referentes a seriados, seus respectivos gêneros, ano de lançamento e nota, sendo armazenados em um banco de dados, onde os mesmos serão disponibilizados para o front-end consumir e otimizar a experiência do usuário ao buscar por séries com melhores notas.

No desenvolver do projeto, foi validado com o cliente o que seria o MÍNIMO PRODUTO VIÁVEL, sendo determinado como uma raspagem simples de um único site de séries, junto de seus respectivos dados. Mostrando apenas as 10 melhores series com maiores notas.

Para o desenvolvimento da aplicação o grupo se subdividiu para organizar as tarefas. Inicialmente seria uma equipe back-end e outra de front-end.

- BACK-END: 
    - RASPAGEM DE DADOS: procuraram cursos gratuitos que ensinassem como raspar dados de um site utilizando Python. A organização deste time foi confusa, já que os dois membros basicamente procuraram as respostas separadamente, assim tomando o dobro de tempo por falta de comunicação. Por fim, um destes alunos conseguiu exito na tarefa e trazendo alguns dados como "teste". Um ajudou o outro após aprender como funcionava tal processo.
    - MANIPULAÇÃO DOS DADOS: alguns destes dados vieram de forma distinta, então a manipulação foi necessária. A atividade foi constituída na retirada de alguns caracteres especiais no nome do filme, gênero e data de lançamento.
    - INSERÇÃO NO BANCO DE DADOS: este tópico exigiu uma ateção maior, pois os membros do grupo não sabiam como os bancos funcionavam e como escolher um que fosse adequado para armazenar dados de um determinado tipo. Com ajuda dos masters e outros colegas mais experientes, foi decidido pelo grupo que o ideal seria um banco de dados não relacional, pois seria armazenado em formato de Json e não em tabelas e colunas como no relacional.
    - MANDAR DADOS DO BANCO PARA O  FRONT-END: neste ponto o front já estava funcionando, mas ainda não consumia dados do banco, eram dados locais no próprio HTML. Novamente alguns colegas mais experientes deram algumas ideias de quais frameworks poderiam utilizar, logo a micro-framework Flask foi escolhida devido o acesso que um dos alunos tinham em uma plataforma de cursos voltados para área da tecnologia.
    
 - FRONT-END:
    - HTML e CSS: os alunos designados para a execução do front-end, começaram a desenvolver a interface gráfica com HTML e CSS, e logo tiveram grandes resultados de como ficaria o projeto em vista do usuário. A área de interação era simples, com uma logo desenvolvida no Canvas e transformada em PNG, uma breve descrição sobre o projeto e, porque foi desenvolvido, e a listagem das 10 series no próprio HTML.
    - PUXAR DADOS DO BANCO: além da framework que o grupo de back-end decidiu utilizar, a equipe de front-end precisaria de JavaScript para manipular os dados como o manuseio de filtros e busca. Este foi um dos processos mais demorados e trabalhosos da equipe, em vista o grau de dificuldade.

Por fim o projeto teve algumas dificuldades, perca de alguns colegas desistentes do curso, porém, em geral, o grupo foi o melhor e único a tirar 10!

## - Tecnologias 
Foi introduzido a linguagem Python para os alunos do 1° semestre, logo projeto deveria seguir com o desenvolvimento com a mesma. Como o a equipe destinguia de conhecimentos sobre desenvolvimento e nomenclaturas como "raspagem de dados", logo a dificuldade na comunicação entre eles e com os professores se manifestou. Por fim realizaram a raspagem de dados com sucesso, utilizando um pacote chamado Beautiful Soup, porém sem armazená-los em algum local. Devido a baixa granularidade dos dados, foi definido o uso de um banco de dados não relacional, armazenariam o nome da serie, genero, data de lançamento e nota em formato de Json; sendo ele o CouchDB. Para fazer a conexão entre os dados e a interface gráfica, foi empregada a framework Flask. E por fim, o frontend foi desenvolvido utilizando HTML, CSS e Javascript para interface e a manipulação dos dados, ato seria a filtragem dos dados mostrados.

- Python:
  Linguagem de programação, desenvolvida para ser simples, fácil de aprender e versátil, logo, para ser utilizá-la em diversas atividades. Sendo ótima para ser a 1° linguagem de se aprender, também é uma das mais utilizadas no mundo e valorizada por poder ser  utilizada em diversas áreas, pode se diferenciar de outras linguagens.
  
 - Beautiful Soup: 
    Pacote Python para análise de documentos HTML e XML. Ele cria uma árvore de análise para páginas analisadas que podem ser usadas para extrair dados de HTML, o que é útil para web scraping.
  
- Flask:
  Micro-framework multiplataforma escrito em Python para gerenciamento no mesmo e disponível em código aberto, oferece um modelo simples para desenvolvimento web. Neste caso lançando as informações do banco de dados até o front-end.
  
- CouchDB:
  Banco de dados NoSQL orientado a documentos. Utiliza JSON como formato de dados e JavaScript como linguagem de consulta. Diferente da maioria  dos outros bancos de dados, seu conteúdo é acessado e modificado através de uma API REST.

- Javacript:
  Linguagem de programação que permite a criação de conteúdos que se atualizam dinamicamente,  controla multimídias, imagens animadas, pesquisas por filtros, entre outros.

## Contribuições individuais

Para desenvolver o back-end do projeto, foi decidido a aproveitamento da linguagem Python e o uso das bibliotecas compativeis com a mesma. Literalmente foi pesquisado por "raspagem de dados" no Google e varios videos e passo-a-passo apontados. O pacote Beautiful Soup era o mais citado dentre os links, logo foi decidido a implemenção. 

Deve ser importado no inicio da classe, conforme a figura a baixo:

![image](https://user-images.githubusercontent.com/55815856/142081595-0be8f770-2b7b-42d1-9b62-60a945e39e26.png)

Declarar o site que deseja consumir:

https://www.imdb.com/search/title/?title_type=tv_series&release_date=1980-01-01,2019-12-31&user_rating=,%27%2710.0&count=250

![gfhadgfadgaidaygafgoaehgouaehg](https://user-images.githubusercontent.com/55815856/141889016-3b3472d9-ccda-4ad0-ba75-1c31019e81ac.PNG)

Selecionando dados relavantes para API consumir:

- Coleta de dados expecificos:

    - Visualização atraves do browser: 
    Botão direito do mouse -> Inspecionar -> Elementos
    ![image](https://user-images.githubusercontent.com/55815856/141889579-7efcc2a8-58ef-470e-9838-3af923fbce9c.png)
 
    - Como os dados são "capturados" pelo pacote Beautiful Soup:
    Utilizando a visualização fornecida pelo browser, pode-se ver o caminho para submeter tal dado.
    ![puxando dados necessarios](https://user-images.githubusercontent.com/55815856/141889757-f9f27295-51e1-454f-a92d-f112f4c435f9.PNG)

Foram encontradas dificuldades em paginar devido a diferença entre URL e quantidade apresentada; raspar outros sites também foi um impedimento pois não foi apresentado metodos ageis de realizar tal processo. Por fim foi decidido manter um unico site com uma unica pagina sendo consumida.

Após extrair os dados, resolvido que os dados deveriam ter os seguintes modificações:
    - O caracter apóstrofo deveria ser retirado dos titulos;
    - As notas deveriam ser numeros quebrados;
    - Alguns generos tinham erro de escrita com "/n", então deveriam ser retirados;
    - Caracteres como números romados, parêntese aperto e fechado, sinal meia-risca deveriam ser retirados das datas de lançamento;
    - Deveriam ser mantidos somente o ano de lançamento, ignorando o ano em que a serie encerou.
        Exemplo: (2007-2012) -> 2007

Foram estudadas as possibilidades de local e como efetuar o armazenamento os dados raspados, chegamos a conclusão de que a melhor ideia seria um banco de daos não relacional, pois não dividiarmos em tantos "pedaços" estes dados. O CouchDB nos foi indicado por alunos mais experientes da mesma faculdade. Para utilizar o banco de dados, só precisaria ter o login e senha declarados no codigo em Python.

- Como autenticar no CouchDB:

![login couchdb](https://user-images.githubusercontent.com/55815856/141023643-b801c2e9-99aa-4a64-a266-1d41c992f9ba.PNG)


- Json no banco de dados:

![image](https://user-images.githubusercontent.com/55815856/142066587-4ac894e6-36b3-446b-9e38-7b083705c0bc.png)


## Aprendizados efetivos
- SCRUM: com o desenvolver deste projeto pude conhecer o scrum e como ele funciona. O papel de cada um e como a comunicação pode ser falha. Cada etapa ou avanço deve ser inspecionado, de modo a identificar se são necessárias possíveis mudanças ou adaptações. Se no sprint anterior forem identificadas necessidades de mudanças é crucial que a equipe Scrum esteja preparado e capacitado para realiza-las. Realizar reuniões para manter a comunicação entre os indiciduos e reportar o andamentos das taks, dificuldades e ou ideias.

- METODOLOGIA ÁGIL: validar a ideia do mínimo produto viável e sempre manter contato com o cliente em todas as sprints, determinando pequenas tarefas distribuídas para um grupo de pessoas conforme a necessidade e facilidade de cada integrante.

- PYTHON: pouco me foi introduzido sobre tal linguagem e reparei que não é tão verbosa quanto presumi que seria. Por ser uma linguagem mais simplificada, não tive tantas dificuldades de entende-la.

    -RASPAGEM DE DADOS: a parte de raspar os dados foi muito interessante e divertida de realizar, a biblioteca Beautiful Soup é bem conhecida e tem vários vídeos de como utilizá-la, me pareceu muito clara na teoria, porém tive um pouco de dificuldade de usá-la por não entender o fluxo do HTML.
    
    - MANIPULAÇÃO DE DADOS: segui uma tilha bem famosa no YouTube e consegui retirar e trocar todos os caracteres especiais dos dados que coletei do IMDB. A trilha é um pouco extensa, tive que dar umas treinadas, mas realmente ajudou muito. Hoje eu indico fortemente o CURSO EM VIDEO do professor Gustavo Guanabara.
    
    - TRANSFORMAR OS DADOS EM JSON: o conceito de criar um modelo (model do projeto) me pareceu abstrato, o que realmente é, mas também é o que estrutura ao dado. Como utilizamos banco de dados não relacional, o Json foi simples.




