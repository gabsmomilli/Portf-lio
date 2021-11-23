# SPC - Inovações no dashboard

## Descrição do projeto:

O Projeto Integrador para o SPC visa estimular o desenvolvimento dos alunos do 3° semestre de Banco de Dados da FATEC de São José dos Campos. Um cliente escolhido pela Fatec, desafiou os alunos do 3° semestre com a proposta de desenvolver um sistema com inovações em seu sistema legado conhecido como SPC. 

A proposta do projeto é a de que um grupo de alunos desenvolva uma aplicação dashboard com interface amigável propondo ao usuário alguma melhoria e ou implementação em seu sistema legado. Não foi requisitado nenhuma linguagem padrão para este projeto, pois o principal objetivo do cliente era o desenvolvimento de uma inovação para seu site.

Os alunos e professores tiveram grande dificuldade de fazerem reuniões com os clientes devido a pandemia e tempo curto do semestre por conta do mesmo, dificultando então a validação dos requisitos, MVC entre outras coisas a serem validadas.

Como se tratava de uma aplicação legado, não foi definido nenhum nome para o projeto.

Foi decidido o uso do banco de dados MySQL por conveniente estudo contínuo do mesmo durante o período. De início o grupo realizou o que seria o rascunho do banco de dados, no qual foi remanejado mais algumas vezes no período. Chegando no seguinte final: 

### COLOCAR FOTO DO DESENHO DO BANCO 

No desenvolver do projeto, foi validado com o cliente o que seria o MÍNIMO PRODUTO VIÁVEL, sendo determinado como um banco de dados enxuto de dados, sendo analisado mais os valores, parcelas e entre outras informações das quais já são informadas no site legado. O cliente disponibilizou uma serie de dados em CSV para fosse aproveitado e consumido no banco de dados. Porém estes mesmos dados estavam com formatações erradas em alguns campos, dados nulos onde não poderiam ser; entretanto foram corrigidas ao desenvolver do projeto.

Para o desenvolvimento da aplicação o grupo se subdividiu para organizar as tarefas. Banco de dados e back-end em uma única pessoa e o fron-end em outra. Esta divisão posta como "grupo" foi devido a desistências do curso logo após a primeira sprint no qual somente o desenho do banco de dados teria sido validado. Com a equipe pequena, não teria como quebrar tanto as tarefas.

A integrante do time de back-end já conhecia um pouco sobre Java com a framework Spring Boot, então por conveniência o grupo optou por utiliza-la.

- BACK-END: 
    - MODELS : definido o modelo exato do banco de dados, a integrante responsável pelo back-end, não teve grandes dificuldades em "replica-la" no padrão Spring. Com os tipos corretos de variáveis, primary key, foreing key e relacionamentos entre tabelas, sendo dos mais variados tipos.
    - PAYLOAD : praticamente uma copia da model, porém somente com dados que não seriam "sensíveis" para o usuário comum, tal como CPF, RG entre outros.
    - BANCO DE DADOS : para a integração com o banco de dados, foi definido no POM as dependências do banco de dados e as definições como nome do banco, porta e senha no APPLICATION. A dificuldade nesta atividade foi entender onde cada informação iria ser determinada, qual arquivo e ordem.
    - REPOSITORY: ministra a ligação a determinada classe do Model com possibilidade de persistir no banco de dados. Lá são definidas as Querys, porém em outro padrão com que os alunos estavam acostumados em desenvolver, pois caso o banco de dados mudasse para Oracle, por exemplo, não teria de ser reformulado muitas linhas de código além do POM com as dependências do novo banco e no APPLICATION com as definições de conexão.
    -  SERVICE : todos os serviços onde estão as regras de negócio, validações e o que mais for preciso. No caso do projeto do SPC, nesta camada que foi criada as validações. 
     entre outras que foram requisitadas neste projeto.
    - CONTROLLER : classe responsável pela preparação de um modelo de Map com dados a serem exibidos pela view e pela escolha da view correta. Basicamente ele é o responsável por controlar as requisições indicando quem deve receber as requisições para quem deve respondê-las. Entregando então pra determinada barra (/tarefa) o que é requisitado como método de requisição HTTP.
    
- BANCO DE DADOS 
    - MYSQL : devido o continuação a matéria Programação de banco de dados, visando a utilização do banco de dados MySQL, o grupo determinou que este seria o ideal, já que poderiam tirar dúvidas com o professor que dava a tal matéria.

## Tecnologias 
A continuação da matéria que referia a linguagem Java para os alunos do 3° semestre, o projeto deveria seguir segundo os integrantes do grupo, com o desenvolvimento com ela. Foi sugerido o uso do framework Spring Boot por uma das integrantes mesmo, pois já estava estudando sobre. Dúvidas e ademais foram tiradas com colegas mais experientes e por pesquisas, pois os alunos ainda não tinham aulas com professores mais especializados em tal framework. Foi decidido a utilização do Spring pois seria reduzido linhas de código que fariam com a linguagem Java pura, além de obter padrões de projetos mais compreensíveis para alunos que estavam começando a ver orientação a objetos.

- Java:
  Linguagem de programação orientada a objetos, provendo diversos frameworks sendo possível a utilização nas aplicações, como por exemplo o Spring, Quarkus, Micronauts, JSF (JavaServer Faces), dentre outros. Java dispõe de vários tipos de dispositivos, como por exemplo: web, mobile, TV Digital, dentre outros. Além disso, há vários cursos gratuitos sobre os mais variados assuntos.
  
 - Spring Bott: 
     Framework Java open source que tem como objetivo facilitar esse processo em aplicações Java. Consequentemente, trazendo mais agilidade para o processo de desenvolvimento, reduzindo linhas de código. Com configurações rápidas, é possível, por exemplo, disponibilizar uma aplicação baseada no Spring MVC, utilizando o Hibernate + JPA.
  
- Hibernate:
  Ferramenta para mapeamento objeto/relacional para ambientes Java, no qual refere-se à técnica de mapeamento de uma representação de dados em um modelo de objetos para um modelo de dados relacional. Cuidando do mapeamento das classes Java para tabelas do banco de dados (e dos tipos de dados Java para os tipos de dados SQL), mas também provê facilidades para consultar e retornar os dados da consulta, e pode reduzir significativamente o tempo de desenvolvimento
  
- JPA:
  Padrão da linguagem Java que descreve uma interface comum para frameworks de persistência de dados. A JPA define um meio de mapeamento objeto-relacional para objetos Java simples e comuns, denominados beans de entidade.
 
- MAVEN:
  Ferramenta de automação de compilação utilizada primariamente em projetos Java. 

## Contribuições individuais

Para desenvolver o back-end do projeto, foi decidido a aproveitamento da linguagem Java e o uso das bibliotecas compatíveis com ela. Foi levado em consideração a indicação de uma integrante do grupo mais experiente. No caso, a técnica Spring MVC com o uso do próprio Spring Boot. 

Criando um projeto Spring Boot:

    - Entrar no link https://start.spring.io/
    
    - Projet: Maven
    
    - Language: Java 
    
    - Spring Boot: 0.0.1-SNAPSHOT (na época)
    
    - Group: test/java/br/gov/sp/fatec/projetointegrador
    
    - Packagin: JAR
    
    - JAVA:  11
    
    - Dependencies: spring-boot-starter-data-jpa
                    spring-boot-starter-web
                    postgresql
                    lombok
                    spring-boot-starter-test
               
 Desenvolvimentos das Models conforme desenhado no banco de dados:
 
    - Seguindo o banco de dados, deve ser declarado o tipo das variáveis equivalente;
    
    - Usar @Entity para o projeto entender que esta classe é uma entidade;
    
    - @Table declarando logo em seguida o nome da tabela no qual esta se referindo;
    
    - @Builder para utilizar o Lombok.
    
 Conexão com o banco de dados no application:
 
    - Declarara por padrão do banco de dados, no caso deste projeto foi utilizado 8081;
    
    - Colocar a url, username e senha da conexão.
    
  Criação dos Repositories: 
  
    - Deixar evidente que é uma interface e extender do JpaRepository, identificando sua model logo em seguida com o tipo da variável id da tabela;
    - Fazer as querys usando @Query no padrão do Spring.
    
   Desenvolvimento da camada Service:
   
    - Utilizar o @Service para o sistema entender que esta é a camada de serviço.
    
    - Colocar anotação @Autowired e logo em seguida o repository desejado;
    
    - Desenvolver as validações necessárias para tal camada.
    
   Adição da camada de Controle:
   
    - No controller, deverá ser incrementado a notação @RestController e @RestMapping, seguido de sua url. Exemplo: @RequestMapping("/projetos");
    
    - Colocar a anotação @Autowired seguida da camada repository desejada;
    
    - Declarar os métodos de busca correspondentes no Repository e colocar a notação do tipo de requerimento HTTP, tal como PUST, GET e DELETE.
   

## Aprendizados efetivos
- AUTONOMIA: Capacidade que um indivíduo tem de tomar decisões com base nas informações que a ele são disponíveis. O projeto para o SPC foi desenvolvido no todo com poucos integrantes, sendo um deles totalmente responsável pelo back-end. Autonomia, proatividade e responsabilidade foram requiridas em todo processo, sendo uma das maiores dificuldades nos alunos iniciantes em programação

- METODOLOGIA ÁGIL: sistema organizacional que contribui para o desenvolvimento de soluções mais eficientes e dinâmicas em grupo, buscando otimizar fluxos de trabalho, melhorar a produtividade de projetos e elevar as perspectivas de sucesso do seu negócio. Aperfeiçoando a produtividade de projetos e aumentar as perspectivas dos resultados. Mantendo como prioridade a satisfação do cliente por meio de entregas de valor contínuas e rápidas. Garantindo a colaboração das partes envolvidas em todo o projeto, por meio de reuniões contínuas.

- SPRING : Java é uma linguagem que demanda muitas linhas de código e a utilização da framework minimiza o mesmo, afim de trazer mais agilidade para o processo de desenvolvimento. O uso de tal ferramenta, proporcionou uma melhor experiencia, organização e entendimento, utilizando o padrão MVC do próprio. Foi um aprendizado efetivo iniciar o projeto em spring, localizar as entidades, criar o mesmo, respository, service e controller, além de proporcionar o melhor entendimento de todo o sistema. Utilização do application para a conexão com o banco de dados e POM com as dependências e configurações necessárias para o mesmo.
