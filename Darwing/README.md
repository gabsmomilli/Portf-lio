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

## - Tecnologias 
Foi introduzido a linguagem Java para os alunos do 2° semestre, logo projeto deveria seguir com o desenvolvimento com a mesma. Foi sujerido o uso da framework Spring Boot por alunos mais experientes do mesmo curso. Dúvidas e ademias foram tiradas tais colegas, pois os alunos ainda não tinham aulas com professores mais expecializados em tal framework. Foi decdido a utilização do Spring pois seria  reduzido linhas de codigo que fariam com a linguagem Java pura, além de obter padrões de projetos mais compreensiveis para alunos que estavam começando a ver orientação a objetos.

- Java:
  Linguagem de programação orientada a objetos, provendo diversas frameworks sendo possivel a utilização nas aplicações, como por exemplo o Spring, Quarkus, Micronauts, JSF (JavaServer Faces), dentre outros. Java dispoe de varios tipod de dispositivos, como por exemplo: web, mobile, TV Digital, dentre outros. Além disso, há varios cursos gratuitos sobre os mais variados assuntos.
  
 - Spring Bott: 
     Framework Java open source que tem como objetivo facilitar esse processo em aplicações Java. Consequentemente, trazendo mais agilidade para o processo de desenvolvimento, reduzindo linhas de codigo. Com configurações rápidas, é possivel, por exemplo, disponibilizar uma aplicação baseada no Spring MVC, utilizando o Hibernate + JPA.
  
- Hibernate:
  Ferramenta para mapeamento objeto/relacional para ambientes Java, no qual refere-se à técnica de mapeamento de uma representação de dados em um modelo de objetos para um modelo de dados relacional. Cuidando do mapeamento das classes Java para tabelas do banco de dados (e dos tipos de dados Java para os tipos de dados SQL), mas também provê facilidades para consultar e retornar os dados da consulta, e pode reduzir significativamente o tempo de desenvolvimento
  
- JPA:
  Padrão da linguagem Java que descreve uma interface comum para frameworks de persistência de dados. A JPA define um meio de mapeamento objeto-relacional para objetos Java simples e comuns, denominados beans de entidade.
 
- MAVEN:
  Ferramenta de automação de compilação utilizada primariamente em projetos Java. 

## Contribuições individuais

Para desenvolver o back-end do projeto, foi decidido a aproveitamento da linguagem Java e o uso das bibliotecas compatíveis com a mesma. Foi levado em consideração a indicação de alunos mais experientes do mesmo curso, na hora de escolher padrões e frameworks do projeto. No caso, a tecnica Spring MVC com o uso do proprio Spring Boot. 

Criando um projeto Spring Boot:
    - Entrar no link https://start.spring.io/
    - Projet: Maven
    - Language: Java 
    - Spring Boot: 0.0.1-SNAPSHOT (na epoca)
    - Group: test/java/br/gov/sp/fatec/projetointegrador
    - Packagin: JAR
    - JAVA:  11
    - Dependencies: spring-boot-starter-data-jpa
                    spring-boot-starter-web
                    postgresql
                    lombok
                    spring-boot-starter-test
               
 Desenvolvimentos das Models conforme desenhado no banco de dados

## Aprendizados efetivos
- SCRUM: com o desenvolver deste projeto é possível informar-se de como funciona o scrum. O papel de cada indivíduo da equipe e como a comunicação pode ser falha. Cada etapa ou avanço deve ser inspecionado, de modo a identificar se são necessárias possíveis mudanças ou adaptações. Se no sprint anterior forem identificadas necessidades de mudanças é crucial que a equipe Scrum esteja preparado e capacitado para realiza-las. Realizar reuniões para manter a comunicação entre os indivíduos e reportar os andamentos das tasks, dificuldades e ou ideias.

- METODOLOGIA ÁGIL: sistema organizacional que contribui para o desenvolvimento de soluções mais eficientes e dinâmicas em grupo, buscando otimizar fluxos de trabalho, melhorar a produtividade de projetos e elevar as perspectivas de sucesso do seu negócio. Aperfeiçoando a produtividade de projetos e aumentar as perspectivas dos resultados. Mantendo como prioridade a satisfação do cliente por meio de entregas de valor contínuas e rápidas. Garantindo a colaboração das partes envolvidas em todo o projeto, por meio de reuniões continuas.

- PYTHON: Devido a simplicidade da linguagem e a demanda de menos código para concluir tarefas básicas quando comparadas a padrões de outras linguagens, sintaxe intuitiva, documentação e passo-a-passo aos montes, bibliotecas gratuitas e por ser uma linguagem interpretada, Python não causa grandes dificuldades em ser utilizada mesmo por desenvolvedores iniciantes. Há muitos cursos bons e gratuitos recheados de conteúdo, basta praticar.

- RASPAGEM DE DADOS: O termo "raspagem de dados" por ser muito técnico, aparenta ser um exercício complexo, o que pode ser para indivíduos iniciantes á programação. Ao           realizar a elaboração do mesmo, muitos relatam ser um experimento interessante e divertido, principalmente quando administrado com a famosa biblioteca Beautiful Soup e disposta com vários vídeos de como utilizá-la. Pode ser relatado dificuldades na utilização caso o desenvolvedor desconheça HTML.
    
- MANIPULAÇÃO DE DADOS: Para realizar a manipulação de dados em Python, basta seguir a documentação do mesmo, contudo, muitos desenvolvedores iniciantes optam por                vídeos. um canal bem famoso por trilhas em Python é o canal Curso em Vídeo do professor Gustavo Guanabara. O curso é extenso, entretanto completo e recheado de                   atividades para o aluno treinar.

- TRANSFORMAR OS DADOS EM JSON: o conceito de criar um modelo (model do projeto) aparenta ser abstrato, o que realmente é, porém é o que estrutura ao dado. Como foi              utilizado banco de dados não relacional, o Json foi simples.
