#  JobNation

## Descrição do projeto:

O Projeto Integrador JobNation visa estimular o desenvolvimento dos alunos do 4° semestre de Banco de Dados da FATEC de São José dos Campos. Cliente "JET SOFT" para que pudéssemos achar uma solução tecnológica para sanar e atender às necessidades do mesmo. Desenvolvendo uma API que possibilita a busca de candidatos a partir de uma vaga, buscando uma contratação veloz e assertiva. Dentre os critérios, deverão ser destaques a segurança e o desempenho da aplicação.

- Requisitos Funcionais:
    Inicializa uma API e se conecta ao/cria BD	
    Executa Requisição de Terceiro	
    Busca candidatos x Nº de conduções do para chegar ao trabalho	
    MATCH Candidato-Vaga	
    Filtra resultado da Busca	
    Busca x critérios de uma 
    
- Requisitos Não Funcionais 
    Regras de segurança da informação	
    Integridade (BD relacional)	
    Flexibilidade quanto aos critérios	
    Regras de performance	
    Documentação
    
### Proposta:
- Busca por localização: número de conduções para chegar ao local de trabalho.

- Busca por diferentes critérios: rota(s) de pesquisa estão sendo desenhadas para propiciar liberdade de consulta ao BD. Nesse passo, a aplicação varrerá currículos já cadastrados e identificará candidato(s) mais adequados à vaga.

Diagrama de caso de uso:

![image](https://user-images.githubusercontent.com/61089745/159176256-013d0b24-b377-4d74-a132-cef3b569b13c.png)

#### FEATURES:

**1) DIAGRAMA-BASE JOBNATION**

![image](https://user-images.githubusercontent.com/61089745/159175589-20bde7c2-7196-4f9b-ab77-7620db50f81d.png)


![image](https://user-images.githubusercontent.com/61089745/159175620-99812ced-b8fa-4a51-9afb-0a8d171d8af0.png)


**2) API JOBNATION**

![image](https://user-images.githubusercontent.com/61089745/159175730-a6778694-b968-4db9-802a-b57b7dac2802.png)

**3) API JOBNATION - NODE-JS - BUSCA QUANTIDADE DE MEIOS DE TRANSPORTES NO GOOGLE MAPS**

![image](https://user-images.githubusercontent.com/61089745/159175766-d0d65974-6f41-492b-9c63-979dd9367347.png)


**4) API JOBNATION - MATCH DE CANDIDATOS (MOST SUITED FOR THE JOB)**

![image](https://user-images.githubusercontent.com/61089745/159175866-5d9f6cb9-8642-4cb4-9841-87ca9060b7e0.png)

**5) SEARCH BY VTn**
![image](https://user-images.githubusercontent.com/61089745/159175929-19d4f5cd-331c-4df4-ad56-dae8f56abe94.png)

**6) JOBNATION's DATABASE**

![image](https://user-images.githubusercontent.com/61089745/159175967-18931a49-e6de-4aea-8de8-92a76986187d.png)

**7) BANCO DE DADOS JOBNATION - FUNCTION BUSCA MÚLTIPLOS CRITÉRIOS COM CURSOR**

![image](https://user-images.githubusercontent.com/61089745/159176040-49f7b721-de66-4767-ad12-a715522ef62f.png)


### Diagrama Entidade-Relacionamento

![image](https://user-images.githubusercontent.com/61089745/159176294-61786526-1747-4945-9dc8-e6a7b0cc23a5.png)


### Inovação:

Criamos o 1o BD com benchmarking no LINKEDIN, subsequentemente alterando o protagonismo para a entidade vaga (VACANCY).

Então, estudamos quais ferramentas servirão aos requisitos (não) funcionais: 

- No BACK-END - Mais de uma linguagem de programação;

- No BD - FUNCTIONS para dar flexibilidade às QUERIES;


### **II - TECNOLOGIAS**:iphone:

![image](https://user-images.githubusercontent.com/61089745/161389515-9616f82e-1054-46e8-9a72-44205be9678a.png)
- Oracle 11g (Sql developer): É um banco de dados popular e relacional, foi usado para criar PROCEDURE PL/SQL: Consulta de candidatos por distância (LAT,LONG); PROCEDURE  de devolução de listas por Múltiplos  Critérios com CURSOR; População do BD com dados fictícios para teste de PERFORMANCE;
![image](https://user-images.githubusercontent.com/61089745/162579889-84c7541e-ae0e-437b-b990-6c8dbd0efb14.png)


![image](https://user-images.githubusercontent.com/61089745/161389576-a377fd09-2c54-40b6-9a7e-c000dd778977.png)
- Java (IntelliJ / Eclipse): Java é uma linguagem de programação orientada a objetos, para desenvolver o backend foi usado os ambientes Eclipse e Intellij para desenvolvimento integrado, escrito em Java. 

![image](https://user-images.githubusercontent.com/61089745/162579991-da2ef388-de98-4e67-80e6-e67fd83420da.png)


![image](https://user-images.githubusercontent.com/61089745/161389691-e18df3bc-2b7d-41bd-b70b-fd59e8d8b266.png)
- Javascript (Node-JS): JavaScript é uma linguagem de programação interpretada estruturada, de script em alto nível. Foi utilizada essa linguagem para fazer a aplicação consumir os dados da API do Google Maps.
![image](https://user-images.githubusercontent.com/61089745/162579708-0e210217-588c-4041-b742-fdb2a1cea274.png)


![image](https://user-images.githubusercontent.com/61089745/161389788-7f4c74dd-fa4b-410a-9e51-376cf8c33817.png)
- Insomnia/POSTMAN: É uma API Client que facilita aos desenvolvedores criar, compartilhar, testar e documentar APIs. Usamos essas API's para testar o backend com as requisições GET, POST, PUT, DELETE e o match entre os candidatos e vagas.


![image](https://user-images.githubusercontent.com/61089745/161389814-314472c1-6046-4348-93ff-c5f1781d0f82.png)
- Git (GitLab): O GitLab é um gerenciador de repositório de software baseado em git, com suporte a Wiki, gerenciamento de tarefas e CI/CD. Guardamos o código do projeto nesse repositório.


![image](https://user-images.githubusercontent.com/61089745/161389851-2c62d470-bb85-479e-9ac2-67c9346a3ee5.png)
- OBS Studio / Kdenlive: É um programa de streaming e gravação gratuito. Foi gravado as telas da aplicação e apresentação usando a ferramenta OBS Studio.


![image](https://user-images.githubusercontent.com/61089745/161389881-fda70645-5197-4c2d-9309-9537b2537a68.png)
- API Google Maps: É um serviço público e gratuito que qualquer pessoa pode usar em seus sites e aplicações. A API foi usada para buscar quantidade de meios de transporte necessárias ao candidato chegar ao local de trabalho.
![image](https://user-images.githubusercontent.com/61089745/162579814-4ef739d0-e3b4-4f8b-bd23-2d733e106e97.png)


### **III - CONTRIBUIÇÕES INDIVIDUAIS**:bow:


Nesse projeto como o foco era o backend e banco de dados não era um requisito ter frontend na aplicação, portanto nas divisões de tasks na equipe escolhi contribuir como de costume a aplicação, ajudando a desenvolver o backend.

Sendo a integrante do grupo com mais conhecimento em Java juntod da framework Spring, dei inicio ao projeto e ensinei aos colegas a desenvolver o mesmo. Com isso, demostrei como utilizo 9 camadas para desenvolvimento das entidades das quais foram definidas.

![image](https://user-images.githubusercontent.com/61089745/164765729-75257564-823f-4901-8cb2-55be55c0759c.png)

 O metodo que eu utilizo chama (MPConConRVS) Model, Payload, Converter, Repository, Validator, Services, Controller.

Fiquei responsável por criar as respectivas camadas e revisar as que meus colegas fizeram.

![image](https://user-images.githubusercontent.com/61089745/164775826-1cccd9f0-f193-4cd6-b864-38682c7a4365.png)

### **IV - APRENDIZADOS EFETIVOS**:closed_book:

**Hard Skills Efetivamente Desenvolvidas:**

- Neste semestre eu apercoei meus conhecimentos em Java.
- Ensinei e revisei codigo de meus colegas.
- Tomei a frente e liderei o back-end.

**Soft Skills Efetivamente Desenvolvidas:**

Aprendi a compartilhar e dividir task no backend, aprendemos mais sobre a comunicação e organização como equipe, colocando em prática o método scrum com Dailys, Revisão e Passagem de Conhecimento.
