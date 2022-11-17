#  HEYSERIES

## Introdução 

Como uma tentativa de introduzir melhor os alunos em problemas atuais do mercado, os professores do curso de Banco de Dados da FATEC de São José dos Campos, decidiram propor um desafio chamado Projeto Integrador, onde ele visa estimular o desenvolvimento dos alunos do 1° semestre do curso.

## Proposta

A proposta do projeto é a de que um grupo de alunos desenvolva uma aplicação utilizando a solução web bot, para resolver o problema proposto pelo próprio grupo. A técnica proposta é "raspagem de dados", dado como um processo de operar uma aplicação para extrair dados valiosos de uma fonte, para utilizá-los a seu favor. Raspagem de conteúdo pode ser então "replicada" ou manipulada conforme o necessário.

## Tecnologias 

- Python: Linguagem de programação, desenvolvida para ser simples, fácil de aprender e versátil, logo, para ser utilizá-la em diversas atividades. Sendo ótima para ser a 1° linguagem de se aprender, também é uma das mais utilizadas no mundo e valorizada por poder ser utilizada em diversas áreas, pode se diferenciar de outras linguagens.
  
 - Beautiful Soup: Pacote Python para análise de documentos HTML e XML. Ele cria uma árvore de análise para páginas analisadas que podem ser usadas para extrair dados de HTML, o que é útil para web scraping.
  
- Flask: Micro framework multiplataforma escrito em Python para gerenciamento no mesmo e disponível em código aberto, oferece um modelo simples para desenvolvimento web. Neste caso lançando as informações do banco de dados até o front-end.
  
- CouchDB: Banco de dados NoSQL orientado a documentos. Utiliza JSON como formato de dados e JavaScript como linguagem de consulta. Diferente da maioria dos outros bancos de dados, seu conteúdo é acessado e modificado através de uma API REST.

- Javacript: Linguagem de programação que permite a criação de conteúdos que se atualizam dinamicamente, controla multimídias, imagens animadas, pesquisas por filtros, entre outros.

## Contribuições individuais

Atuei no desenvolvimento back-end do projeto, com a linguagem Python, utilizando o pacote pacote Beautiful Soup para extração e raspagem de dados

Deve ser importado no inicio da classe, conforme a figura a baixo:

<details>
  <summary>Click aqui pra visualizar</summary>
  
  ```js
  from bs4 imoprt BeautifulSoup, ResultSet
  ```
</details>

Declarar o site que deseja consumir:

https://www.imdb.com/search/title/?title_type=tv_series&release_date=1980-01-01,2019-12-31&user_rating=,%27%2710.0&count=250

<details>
  <summary>Click aqui pra visualizar</summary>
  
  ```js
  result = requests.get('https://www.imdb](https://www.imdb.com/search/title/?title_type=tv_series&release_date=1980-01-01,2019-12-31&user_rating=,%27%2710.0&count=250')
  ```
</details>

Selecionando dados relevantes para API consumir:

Visualização através do browser: 
    
    Botão direito do mouse -> Inspecionar -> Elementos
    
    <details>
  <summary>Click aqui pra visualizar</summary>
  <br>
   <img style="border-radius: 50%;" src="https://user-images.githubusercontent.com/55815856/141889579-7efcc2a8-58ef-470e-9838-3af923fbce9c.png" width="500px;" alt=""/>
</details>
 
 Como os dados são "capturados" pelo pacote Beautiful Soup:
    
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

Autenticando no CouchDB:

<details>
  <summary>Click aqui pra visualizar</summary>
  
  ```js
  auth = ('couchdb', 'couchdb')
  ```
</details>


- Json no banco de dados:

![image](https://user-images.githubusercontent.com/55815856/142066587-4ac894e6-36b3-446b-9e38-7b083705c0bc.png)


## Aprendizados efetivos
- SCRUM: com o desenvolver deste projeto é possível informar-se de como funciona o scrum. O papel de cada indivíduo da equipe e como a comunicação pode ser falha. Cada etapa ou avanço deve ser inspecionado, de modo a identificar se são necessárias possíveis mudanças ou adaptações. Se no sprint anterior forem identificadas necessidades de mudanças é crucial que a equipe Scrum esteja preparado e capacitado para realiza-las. Realizar reuniões para manter a comunicação entre os indivíduos e reportar os andamentos das tasks, dificuldades e ou ideias.

- METODOLOGIA ÁGIL: sistema organizacional que contribui para o desenvolvimento de soluções mais eficientes e dinâmicas em grupo, buscando otimizar fluxos de trabalho, melhorar a produtividade de projetos e elevar as perspectivas de sucesso do seu negócio. Aperfeiçoando a produtividade de projetos e aumentar as perspectivas dos resultados. Mantendo como prioridade a satisfação do cliente por meio de entregas de valor contínuas e rápidas. Garantindo a colaboração das partes envolvidas em todo o projeto, por meio de reuniões continuas.

- PYTHON: Devido a simplicidade da linguagem e a demanda de menos código para concluir tarefas básicas quando comparadas a padrões de outras linguagens, sintaxe intuitiva, documentação e passo-a-passo aos montes, bibliotecas gratuitas e por ser uma linguagem interpretada, Python não causa grandes dificuldades em ser utilizada mesmo por desenvolvedores iniciantes. Há muitos cursos bons e gratuitos recheados de conteúdo, basta praticar.

- RASPAGEM DE DADOS: O termo "raspagem de dados" por ser muito técnico, aparenta ser um exercício complexo, o que pode ser para indivíduos iniciantes á programação. Ao           realizar a elaboração do mesmo, muitos relatam ser um experimento interessante e divertido, principalmente quando administrado com a famosa biblioteca Beautiful Soup e disposta com vários vídeos de como utilizá-la. Pode ser relatado dificuldades na utilização caso o desenvolvedor desconheça HTML.
    
- MANIPULAÇÃO DE DADOS: Para realizar a manipulação de dados em Python, basta seguir a documentação do mesmo, contudo, muitos desenvolvedores iniciantes optam por                vídeos. um canal bem famoso por trilhas em Python é o canal Curso em Vídeo do professor Gustavo Guanabara. O curso é extenso, entretanto completo e recheado de                   atividades para o aluno treinar.

- TRANSFORMAR OS DADOS EM JSON: o conceito de criar um modelo (model do projeto) aparenta ser abstrato, o que realmente é, porém é o que estrutura ao dado. Como foi              utilizado banco de dados não relacional, o Json foi simples.
