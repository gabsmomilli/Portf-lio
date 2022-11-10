## FATEC & IONIC HEALTH - EDUCALYTICS:mortar_board:

### **I - RESUMO DO PROJETO**:page_facing_up: 

Neste quinto Projeto Integrador a FATEC trouxe o Cliente "IONIC HEALTH" para que pudéssemos achar uma solução tecnológica para sanar e atender às necessidades do cliente. 

O cliente visa indicadores e avaliar o uso e gerenciamento de sua plataforma de cursos, buscando os alunos que estão com boa frequência nas aulas, que entra em contato por chat para sanar dúvidas e avaliação das aulas dadas.

Com base nesse briefing, solicita uma plataforma funcional com capacidade analítica, com dashboards, histórico de chat e armazenamento desses dados. Para a realização da análise deverá ter especialmente:


* Ativação: Quantos usuários ativos (aluno/colaboradores) na plataforma legado;
* Engajamento: Conhecer o número de usuários, tipos, seu comportamento (matrícula, curso, disciplina, participação);
* Desempenho: qual o aproveitamento do aluno(nota atingida) e do professor (andamento da turma);
* Participação x taxas de conclusão x desempenho dos alunos/colaboradores;
* Avaliação de reação: quanto ao conteúdo apresentado, experiência do aluno/colaborador durante o curso;
* Registro do tempo de participação no curso;
* Guardar logs e histórico das conversas do chat;


#### Requisitos Funcionais


| Functional Requirements                                                 | Reference |
|------------------------------------------------------------------------|--------|
| Dashboard: apresentar dados ao cliente (via backend e banco de dados 01 relacional)        | RF01   | 1          | 1      |
| Continuous Integration | RF02   | 1          | 4      |
| Tratar Logs| RF03   | 1          | 2      |
| Tratar Chats   | RF04  | 1          | 3     |
| Acumular dados históricos tratados e gerar inteligência para o client, via DASHBOARD |RF05	| 1	| 4




#### Requisitos Não Funcionais


| Non-functional Requirements                            | Reference | 
|------------------------------------------------------|--------|
| Regras de segurança da informação         | RNF01  |
| Regras de privacidade              | RNF02  |
| Documentação | RNF03  |
| Escalabilidade  | RNF04  |
| Facilidade de Uso | RNF05 |



### Proposta:

Desenvolver uma aplicação capaz de buscar dados de uma fonte externa, ou seja, uma aplicação legada (chamado Skillshare), para fornecer aos usuários informações suficientes para administrar uma instituição de ensino.

Os dados são produzidos através do uso regular de uma plataforma de e-learning. Assim, um histórico de uso, incluindo interação do usuário via chats e logs do sistema, atribuições, desempenho dos alunos e satisfação do usuário devem ser extraídos, compilados e apresentados aos nossos clientes.

Eventualmente, a Educalytics deve ser capaz de transmitir o comportamento dos usuários de aplicações legados e fornecer à instituição de ensino inteligência suficiente, apoiando seu processo de tomada de decisão.

Seguindo essas premissas listadas acima, a Educalytics apresentará uma GUI por meio de um DASHBOARD com os dados mais importantes do ponto de vista da instituição de ensino.

#### Diagrama de Casos de Uso:

![image](https://user-images.githubusercontent.com/61089745/159184157-6fff7a22-2156-4560-a6f5-bcabda70e1ac.png)


#### FEATURES:

1- ARQUITETURA DO EDUCALYTICS

![image](https://user-images.githubusercontent.com/61089745/159179873-f5a8d7c4-46a5-4a91-91a1-e0e801627a9f.png)

2- FRONTEND;

2.1- DASHBOARD (MVP);

![image](https://user-images.githubusercontent.com/61089745/159179889-472655a1-6d5e-42a4-9cb2-eea4712c2dea.png)

2.2- TELA DE LOGIN (COM CRIPTOGRAFIA "bcript");

![image](https://user-images.githubusercontent.com/61089745/159179961-dcf5594d-12dc-478b-b458-35f7781dd083.png)

![image](https://user-images.githubusercontent.com/61089745/159179972-f344d07b-364b-4aed-9f0d-b81657fcc252.png)


2.3- SOLICITAÇÃO USANDO TOKEN ÚNICO;

![image](https://user-images.githubusercontent.com/61089745/164943290-850f703d-27b1-4854-b3dd-32f75d35b41d.png)

2.4- INTEGRAÇÃO CONTÍNUA;

![image](https://user-images.githubusercontent.com/61089745/159180157-a0b5818d-0427-46b8-acdc-74a18df75e9c.png)

![image](https://user-images.githubusercontent.com/61089745/159180165-7dd29c0b-2c8b-45b2-8065-21603f725f8c.png)

![image](https://user-images.githubusercontent.com/61089745/159180282-37075ff4-a3e2-4caf-a144-ddcf97ee4a75.png)

![image](https://user-images.githubusercontent.com/61089745/159180717-f73588d8-e928-4b77-bf04-f0061acfe084.png)


2.5- APRESENTAÇÃO DOS RESULTADOS DA PARTICIPAÇÃO DOS ALUNOS VIA GRÁFICOS NO PAINEL;
![image](https://user-images.githubusercontent.com/61089745/159181410-6229d04f-c7df-4b15-8979-61d8e15d9efd.png)


2.6- RESULTADOS EM CADA AULA;

![image](https://user-images.githubusercontent.com/61089745/159182151-5df61b9d-3654-4446-8038-e1b2e1abb040.png)

3-  BACKEND - AS 8 CAMADAS (MPConConRVSC).

Model, 
Payload, 
Config, 
Converter, 
Repository, 
Validator, 
Services, 
Controller.

![image](https://user-images.githubusercontent.com/61089745/159182772-fe3f1484-3eb9-4c07-96d6-aaa1e9545245.png)

3.1- BACKEND - VALIDAÇÃO (usuário e senha).

![image](https://user-images.githubusercontent.com/61089745/159183570-aa8ac41f-46a5-4dac-a5e7-e7f38a69a303.png)

3.2- BACKEND - ACESSO A BANCO DE DADOS

![image](https://user-images.githubusercontent.com/61089745/159183668-f5723b53-0a9a-42ce-9114-4d4a4a87f344.png)

3.3- BACKEND - ETL.

![image](https://user-images.githubusercontent.com/61089745/159183744-7e2c9c21-0b80-4aef-8874-6ec2d75805da.png)


3.3.1- BACKEND - ETL TIME DIMENSION.

![image](https://user-images.githubusercontent.com/61089745/159183767-2cab25de-25d6-4c70-a051-04a98087495f.png)

4- BASE DE DADOS DO EDUCALYTICS (RELACIONAL)

4.1- MODELO LÓGICO

![image](https://user-images.githubusercontent.com/61089745/159183917-ca07238a-9570-4461-917f-481f6088cb52.png)

4.2- MODELO DE RELACIONAMENTO DE ENTIDADE

![image](https://user-images.githubusercontent.com/61089745/159183927-84af1794-bd8d-49a8-a4cc-b9727d9109e6.png)

4.3 PARTICIPAÇÃO DO DATAMART - EXTRAÇÃO DE DADOS DO MONGO DB

![image](https://i.ibb.co/ssS7yBm/EXTRACAO-MONGO-DB.png)


5- BASE DE DADOS(NÃO RELACIONAL)

![image](https://i.ibb.co/pXyJ1qQ/DATAMART-02-ENGAJAMENTO.png)

5.1- PARTICIPAÇÃO DO DATAMART - COLETA DE MENSAGENS

![image](https://i.ibb.co/NNj5jnf/COLLECTION-MESSAGES.png)

5.2- REGISTRO DE CHAT+LOGS INSERIDO NO MONGO DB CLOUD
![image](https://i.ibb.co/WxhRFtm/DADOS-DO-CHAT-E-DOS-LOGS.png)


### Inovação
Criamos o 1º BD a partir dos dados considerados necessários, a partir dos requisitos do cliente e da aplicação legado (Skillshare).  Subsequentemente, alteramos o protagonismo para as entidades que envolvem a ligação entre Alunos, Professores e Disciplina.
Então, estudamos quais ferramentas servirão aos requisitos (não) funcionais:


- No FRONTEND - criptografia e token;
- No BACKEND - arquitetura em oito camadas;
- No BANCO DE DADOS 01 (RELACIONAL) - Primeira versão com todos os dados necessários (será decomposto);
- No BANCO DE DADOS 02 (NÃO-RELACIONAL) - Receberá tabelas do BD01, segundo critérios de performance;
- Distribuição dos BD - Se necessária a clusterização / fragmentação;
- No DATA WAREHOUSE - Ferramentas de relatório, de ETL no terceiro banco de dados.



### **II - TECNOLOGIAS**:iphone:

![image](https://user-images.githubusercontent.com/61089745/161389576-a377fd09-2c54-40b6-9a7e-c000dd778977.png)
- Java: É uma linguagem de programação orientada a objetos. Foi utilizado essa linguagem para o desenvolvimento do backend da aplicação.

![image](https://user-images.githubusercontent.com/61089745/161391318-463c5040-eaab-4d45-9ff2-6dfcf4f81991.png)
- IntelliJ/Eclipse: Java é uma linguagem de programação orientada a objetos, para desenvolver o backend foi usado os ambientes Eclipse e Intellij para desenvolvimento integrado, escrito em Java. 

![image](https://user-images.githubusercontent.com/61089745/161391346-b359a7ca-73c9-460d-8814-b52cc435d222.png)
- VS CODE: O Visual Studio Code é um editor de código-fonte desenvolvido pela Microsoft para Windows, Linux e macOS. Foi usado para rodar a aplicação frontend e backend no ambiente de alguns integrantes do grupo.

![image](https://user-images.githubusercontent.com/61089745/161389691-e18df3bc-2b7d-41bd-b70b-fd59e8d8b266.png)
- JavaScript/NodeJS: JavaScript é uma linguagem de programação interpretada estruturada, de script em alto nível com tipagem dinâmica fraca e multiparadigma. Juntamente com HTML e CSS. Foi usada essa linguagem para desenvolver o frontend.

![image](https://user-images.githubusercontent.com/61089745/161391408-584a934b-73f9-4c74-b463-a8b2d9b71ee0.png)
- MicrosoftSQLServer: O Microsoft SQL Server é um sistema gerenciador de Banco de dados relacional desenvolvido pela Sybase em parceria com a Microsoft. Foi usado para o desenvolvimento do ETL.

![image](https://user-images.githubusercontent.com/61089745/161391358-e87e6d1a-63ec-40bc-b19d-422df7414cea.png)
- MySQL: O MySQL é um sistema de gerenciamento de banco de dados, que utiliza a linguagem SQL como interface. Foi usado para o desenvolvimento do banco relacional da aplicação.

![image](https://user-images.githubusercontent.com/61089745/161389774-0acaa3e2-478b-444f-aeba-2f6ad4fec469.png)
- React: O React é uma biblioteca JavaScript de código aberto com foco em criar interfaces de usuário em páginas web.

![image](https://user-images.githubusercontent.com/61089745/161389788-7f4c74dd-fa4b-410a-9e51-376cf8c33817.png)
- Insomnia/Postman: É um API Client que facilita aos desenvolvedores criar, compartilhar, testar e documentar APIs. Utizada para testar o GET, PUT, POST e DELETE das classes controllers da aplicação.

![image](https://user-images.githubusercontent.com/61089745/161389814-314472c1-6046-4348-93ff-c5f1781d0f82.png)
- GitLab/GitFlow: O GitLab é um gerenciador de repositório de software baseado em git, com suporte a Wiki, gerenciamento de tarefas e CI/CD. Foi usado para armazenar o código do projeto e desenvolver o CI/CD GitFLow da aplicação.

![image](https://user-images.githubusercontent.com/61089745/161391438-d192b5d7-b7b2-4acc-89f8-e4db42c70c97.png)
- MongoDB: É um software de banco de dados orientado a documentos livre, de código aberto e multiplataforma, escrito na linguagem C++. Classificado como um programa de banco de dados NoSQL, o MongoDB usa documentos semelhantes a JSON com esquemas. Foi usado para armazenar os logs do chat da aplicação legada no banco não relacional.

![image](https://user-images.githubusercontent.com/61089745/161389851-2c62d470-bb85-479e-9ac2-67c9346a3ee5.png)
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

Aprimorei os conhecimentos em back-end utilizando um novo metodo orientado pelos professores, e desenvolvi a conexão entre a API e dois bancos diferentes.

Através dos conhecimentos compartilhados entre o grupo aprendi sobre a ferramenta ETL;

**Soft Skills Efetivamente Desenvolvidas:**

Continuei desenvolvendo e melhorando a comunicação, trabalho em equipe e ajuda mútua;

Tivemos que sair da nossa zona de conforto e buscar novos conhecimentos através de cursos extras e ajuda dos professores para conseguir desenvolver novas features da aplicação em que não tinhamos vivência;

Conseguimos ter a inteligência e resiliência para construir um bom planejamento. O método Scrum nos ajudou a cumprir todas as entregas e sprints do projeto.
