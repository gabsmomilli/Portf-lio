# DARWING

## Introdução

A FATEC junto com a empresa Necto System, propuseram para os alunos o desafio da criação de um software que visa estimular o desenvolvimento e mais ativamente a interaçao com as materias do 2º semetre de Banco de Dados da FATEC de São José dos Campos.

## Proposta

A proposta do projeto é a de que um grupo de alunos desenvolva uma aplicação administrativa de afazeres, sendo para uma única pessoa ou até mesmo para uma empresa. O padrão de projeto proposto é MVC em Java utilizando a framework Spring Boot, oferecendo mais agilidade para o processo de desenvolvimento, dado que os desenvolvedores conseguem reduzir o tempo gasto com as configurações iniciais.
 
## Contribuições individuais 

Neste projeto a quipe estava com equipe reduzida, deixando somente eu com o back-end para desenvolver. Dei inicio aos meus estudos com a linguagem Java utilizando a framework Spring Boot. Crei a conexão do nosso banco de dados MySQL, e após a definição de como seria o nosso modelo de banco de dados, criei as models referente as entidades, em seguida iniciei o desenvolvimento das camadas necessarias, sendo elas: repository, service e controller.

Na camada de repository ministrei a ligação a determinada classe do Model com possibilidade de persistir no banco de dados. Defini as Querys em um padrão diferenciado para caso mudasse o banco para Oracle, por exemplo, não teria de ser reformulado muitas linhas de código além do POM com as dependências do novo banco e no APPLICATION com as definições de conexão.
Ja no service é onde se encontra as regras de negócio, validações e o que mais for preciso. No caso do Darwing, nesta camada que foi criada as validações, como:
        - se haviam campos nulos;
        - se o desenvolvedor já não estava cadastrado;
        - carga horaria maior que 0 horas. 
O controller é a classe responsável pela preparação de um modelo de Map com dados a serem exibidos pela view e pela escolha da view correta. Basicamente ele é o responsável por controlar as requisições indicando quem deve receber as requisições para quem deve respondê-las. Entregando então pra determinada barra (/tarefa) o que é requisitado como método de requisição HTTP.

## Tecnologias 

- Java: Linguagem de programação orientada a objetos, provendo diversos frameworks sendo possível a utilização nas aplicações, como por exemplo o Spring, Quarkus, Micronauts, JSF (JavaServer Faces), dentre outros. Utilizada para consumir e manipular os dados vindos do banco de dados MySQL.
  
 - Spring Bott: Framework Java open source que tem como objetivo facilitar esse processo em aplicações Java. Consequentemente, trazendo mais agilidade para o processo de desenvolvimento, reduzindo linhas de código. Urilizada para agilizar e padronizar o desenvolvimento do projeto.
  
- Hibernate:
  Ferramenta para mapeamento objeto/relacional para ambientes Java. Utilizada no mapaeamento de uma representação de dados em um modelo de objetos para um modelo de dados relacional. Cuidando do mapeamento das classes Java para tabelas do banco de dados.
  
- JPA:
  Padrão da linguagem Java que descreve uma interface comum para frameworks de persistência de dados. A JPA define um meio de mapeamento objeto-relacional para objetos Java simples e comuns, denominados beans de entidade.
 
- MAVEN:
  Ferramenta de automação de compilação utilizada primariamente em projetos Java. 

## Aprendizados efetivos

### Hard Skills
- Iniciei meus estudos com a linguagem Java;
- Iniciei meus estudos com a framework Spring;
- Iniciei meus estudos com a framework Hibernate.

### Soft Skills
- Autonimia;
- Metodologia Agil;
- Comunicaçao.
