# Inovações no dashboard

## Introdução

No 3º periodo do curso de Banco de dados da FATEC de São José dos Campos se aliou a empresa SPC para propor um problema a ser solucionado pelos alunos do semestre.

## Proposta

A proposta do projeto é o desenvolvimento de uma aplicação dashboard com interface amigável propondo ao usuário alguma melhoria e ou implementação em seu sistema legado. 

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

## Contribuições individuais

Neste projeto permaneci no desenvolvimento do back-end. Aprimorei meus conhecimentos na linguagem Java com a framework Spring. Conectei a API com o banco de dados e os preparei para o front-end consumir.

## Tecnologias

- Java: Linguagem de programação orientada a objetos, provendo diversos frameworks sendo possível a utilização nas aplicações. Utilizada para consumir e manipular os dados vindos do banco de dados MySQL.
  
- Spring Bott: Framework Java open source que tem como objetivo facilitar esse processo em aplicações Java. Consequentemente, trazendo mais agilidade para o processo de desenvolvimento, reduzindo linhas de código. Urilizada para agilizar e padronizar o desenvolvimento do projeto.
  
- Hibernate: Ferramenta para mapeamento objeto/relacional para ambientes Java. Utilizada no mapaeamento de uma representação de dados em um modelo de objetos para um modelo de dados relacional. Cuidando do mapeamento das classes Java para tabelas do banco de dados.

- JPA: Padrão da linguagem Java que descreve uma interface comum para frameworks de persistência de dados. A JPA define um meio de mapeamento objeto-relacional para objetos Java simples e comuns, denominados beans de entidade.

- MAVEN: Ferramenta de automação de compilação utilizada primariamente em projetos Java.

## Aprendizados efetivos

### Hard Skills

- Realizei a conexaõ do banco de dados MySQL com Hibernate;
- Aprimorei meus conhecimentos em Java junto a framework Spring;
- Preparei os dados para o front-end consumir.

### Soft Skills

- Autonomia;
- Metodologia Agil;
- Comunicação;
- Liderança;
- Scrum.
