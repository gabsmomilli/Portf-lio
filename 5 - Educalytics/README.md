# EDUCALYTICS

## Introdução

A empresa Ionic Health propôs um desafio acadêmico para os alunos do 5º semestre do curso de Banco de Dados da FATEC-SJC, a fim de estimular o desenvolvimento das matérias do período, os preparando para o mercado de trabalho, e encontrar uma solução tecnologica para sanar e atender às necessidades do cliente. 

## Proposta
O objetivo da parceria era o desenvolvimento de uma API que realizasse o desenvolvimento de indicadores e avaliar o uso e gerenciamento de sua plataforma de cursos, buscando os alunos que estão com boa frequência nas aulas, entrar em contato por chat para sanar dúvidas e avaliação das aulas dadas. 

A Ionic Health solicitou uma plataforma funcional com capacidade analítica, com dashboards, histórico de chat e armazenamento desses dados. Para a realização da análise deverá ter especialmente:


* Ativação: quantos usuários ativos (aluno/colaboradores) na plataforma legado;
* Engajamento: conhecer o número de usuários, tipos, seu comportamento (matrícula, curso, disciplina, participação);
* Desempenho: qual o aproveitamento do aluno(nota atingida) e do professor (andamento da turma);
* Participação: x taxas de conclusão x desempenho dos alunos/colaboradores;
* Avaliação de reação: quanto ao conteúdo apresentado, experiência do aluno/colaborador durante o curso;
* Registro do tempo de participação no curso;
* Guardar logs e histórico das conversas do chat;


### Requisitos Funcionais


| Functional Requirements                                                 | Reference |
|------------------------------------------------------------------------|--------|
| Dashboard: apresentar dados ao cliente (via backend e banco de dados 01 relacional)        | RF01   | 1          | 1      |
| Continuous Integration | RF02   | 1          | 4      |
| Tratar Logs| RF03   | 1          | 2      |
| Tratar Chats   | RF04  | 1          | 3     |
| Acumular dados históricos tratados e gerar inteligência para o client, via DASHBOARD |RF05	| 1	| 4




### Requisitos Não Funcionais


| Non-functional Requirements                            | Reference | 
|------------------------------------------------------|--------|
| Regras de segurança da informação         | RNF01  |
| Regras de privacidade              | RNF02  |
| Documentação | RNF03  |
| Escalabilidade  | RNF04  |
| Facilidade de Uso | RNF05 |


#### Diagrama de Casos de Uso:

<details>
  <summary>Click aqui pra visualizar</summary>
  <br>
   <img style="border-radius: 50%;" src="https://user-images.githubusercontent.com/61089745/159184157-6fff7a22-2156-4560-a6f5-bcabda70e1ac.png" width="500px;" alt=""/>
</details>


### TECNOLOGIAS

- Java: É uma linguagem de programação orientada a objetos. Foi utilizado essa linguagem para o desenvolvimento do backend da aplicação.

- IntelliJ/Eclipse: Java é uma linguagem de programação orientada a objetos, para desenvolver o backend foi usado os ambientes Eclipse e Intellij para desenvolvimento integrado, escrito em Java. 

- VS CODE: O Visual Studio Code é um editor de código-fonte desenvolvido pela Microsoft para Windows, Linux e macOS. Foi usado para rodar a aplicação frontend e backend no ambiente de alguns integrantes do grupo.

- JavaScript/NodeJS: JavaScript é uma linguagem de programação interpretada estruturada, de script em alto nível com tipagem dinâmica fraca e multiparadigma. Juntamente com HTML e CSS. Foi usada essa linguagem para desenvolver o frontend.

- MicrosoftSQLServer: O Microsoft SQL Server é um sistema gerenciador de Banco de dados relacional desenvolvido pela Sybase em parceria com a Microsoft. Foi usado para o desenvolvimento do ETL.

- MySQL: O MySQL é um sistema de gerenciamento de banco de dados, que utiliza a linguagem SQL como interface. Foi usado para o desenvolvimento do banco relacional da aplicação.

- React: O React é uma biblioteca JavaScript de código aberto com foco em criar interfaces de usuário em páginas web.

- Insomnia/Postman: É um API Client que facilita aos desenvolvedores criar, compartilhar, testar e documentar APIs. Utizada para testar o GET, PUT, POST e DELETE das classes controllers da aplicação.

- GitLab/GitFlow: O GitLab é um gerenciador de repositório de software baseado em git, com suporte a Wiki, gerenciamento de tarefas e CI/CD. Foi usado para armazenar o código do projeto e desenvolver o CI/CD GitFLow da aplicação.

- MongoDB: É um software de banco de dados orientado a documentos. Foi usado para armazenar os logs do chat da aplicação legada no banco não relacional.

- OBS Studio/Kdenlive: É um programa de streaming e gravação gratuito. Usada para gravar vídeos das sprints.

### **III - CONTRIBUIÇÕES INDIVIDUAIS**:bow:

Nesse projeto estavámos com uma equipe reduzida perto dos outros grupos da turma, o Projeto Integrador foi o mais desafiador com requisitos complexos e exigindo conhecimentos específicos para compor a aplicação. Com isso, decidimos dividir a equipe deixando os integrantes assumir as tarefas que mais tinham conhecimento para ganharmos tempo e posteriormente dedicarmos em correr atrás das features que não tínhamos habilidades.

Portanto, optei por continuar no desenvolvimento do back-end da aplicação criando as entidades e demais camadas do sistema.

Desenvolvi no back-end as classes para integração com o front-end e para o ETL.

![image](https://user-images.githubusercontent.com/61089745/164789664-7ac7c21b-e7b5-47f4-9137-2220ed495ff9.png)


Implementei Testes Unitários para cobertura do código e integração com o CI;

![image](https://user-images.githubusercontent.com/61089745/164792269-6d8a12bf-e999-4915-82d4-63926b337d0e.png)

Implementei dois bancos de dados no sistema, sendo um relacional e outro não relacional 

<COLOCAR IMAGEM>


### **IV - APRENDIZADOS EFETIVOS**:closed_book:

**Hard Skills Efetivamente Desenvolvidas:**

Este foi o Projeto Integrador mais desafiador por ter a equipe reduzida e implementação de varias tecnologias e soluções a serem aplicadas.

Aprimorei os conhecimentos em back-end utilizando um novo método orientado pelos professores, e desenvolvi a conexão entre a API e dois bancos diferentes.

Através dos conhecimentos compartilhados entre o grupo aprendi sobre a ferramenta ETL;

Soft Skills Efetivamente Desenvolvidas:

Continuei desenvolvendo e melhorando a comunicação, trabalho em equipe e ajuda mútua;

Tivemos que sair da nossa zona de conforto e buscar novos conhecimentos através de cursos extras e ajuda dos professores para conseguir desenvolver novas features da aplicação em que não tínhamos vivência;

Conseguimos ter a inteligência e resiliência para construir um bom planejamento. O método Scrum nos ajudou a cumprir todas as entregas e sprints do projeto.
