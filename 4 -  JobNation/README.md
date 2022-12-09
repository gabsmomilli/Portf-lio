#  JOBNATION

## Introdução

A parceira da FATEC junto a empresa JET SOFT, proporcionou aos alunos do 4° semestre do curso de Banco de Dados, o desafio onde eles deveriam apresentar uma solução tecnológica para sanar e atender às necessidades do mesmo, visando um match entra candidato e vaga.
    
## Proposta:

A proposta desse semstre era o desenvolvimento uma API que possibilita a busca de candidatos a partir de uma vaga, buscando uma contratação veloz e assertiva. Dentre os critérios, deveriam ser destaques a segurança e o desempenho da aplicação.

Esta API deve realizar a busca por localização: número de conduções para chegar ao local de trabalho; busca por diferentes critérios: rota(s) de pesquisa estão sendo desenhadas para propiciar liberdade de consulta ao BD. Nesse passo, a aplicação varrerá currículos já cadastrados e identificará candidato(s) mais adequados à vaga.

## Contribuições individuais 

Nesse projeto como o foco era o back-end e banco de dados não era um requisito ter frontend na aplicação, portanto nas divisões de tasks na equipe escolhi contribuir como de costume a aplicação, ajudando a desenvolver o backend.

Sendo a integrante do grupo com mais conhecimento em Java junto da framework Spring, dei inicio ao projeto e ensinei aos colegas a desenvolver o mesmo. Com isso, demostrei como utilizo 9 camadas para desenvolvimento das entidades das quais foram definidas.

<details>
  <summary>Click aqui pra visualizar</summary>
  <br>
   <img style="border-radius: 50%;" src="https://user-images.githubusercontent.com/61089745/164765729-75257564-823f-4901-8cb2-55be55c0759c.png" width="500px;" alt=""/>
</details>

 O metodo que eu utilizo chama (MPConConRVS) Model, Payload, Converter, Repository, Validator, Services, Controller.

Fiquei responsável por criar as respectivas camadas e revisar as que meus colegas fizeram.
<details>
  <summary>Click aqui pra visualizar</summary>
  <br>
   <img style="border-radius: 50%;" src="https://user-images.githubusercontent.com/61089745/164775826-1cccd9f0-f193-4cd6-b864-38682c7a4365.png" width="500px;" alt=""/>
</details>

## Tecnologias

- Oracle 11g (Sql developer): É um banco de dados popular e relacional, foi usado para criar PROCEDURE PL/SQL: Consulta de candidatos por distância (LAT,LONG); PROCEDURE  de devolução de listas por Múltiplos  Critérios com CURSOR; População do BD com dados fictícios para teste de PERFORMANCE;

- Java (IntelliJ / Eclipse): Java é uma linguagem de programação orientada a objetos, para desenvolver o back-end foi usado os ambientes Eclipse e Intellij para desenvolvimento integrado, escrito em Java. 

- Javascript (Node-JS): JavaScript é uma linguagem de programação interpretada estruturada, de script em alto nível. Foi utilizada essa linguagem para fazer a aplicação consumir os dados da API do Google Maps.

- Insomnia/POSTMAN:  É uma API Client que facilita aos desenvolvedores criar, compartilhar, testar e documentar APIs. Usamos essas API's para testar o back-end com as requisições GET, POST, PUT, DELETE e o match entre os candidatos e vagas.

- GitLab: Gerenciador de repositório de software baseado em git, com suporte a Wiki, gerenciamento de tarefas e CI/CD. Guardamos o código do projeto nesse repositório.

- OBS Studio / Kdenlive: É um programa de streaming e gravação gratuito. Foi gravado as telas da aplicação e apresentação usando a ferramenta OBS Studio.

- API Google Maps: É um serviço público e gratuito que qualquer pessoa pode usar em seus sites e aplicações. A API foi usada para buscar quantidade de meios de transporte necessárias ao candidato chegar ao local de trabalho.

## Aprendizados efetivos

### Hard Skills 

- Neste semestre eu aperfeiçoei meus conhecimentos em Java;
- Iniciei meus estudos com branching;
- Utilizei pela primeira vez o banco de dados Oracle integrado com API.

### Soft Skills
 - Autonomia: Já estava familiarizada com as tecnologias utilizadas, então não tive grandes dificuldades para realizar minhas tarefas;
 - Liderança do back-end: como era o membro da equipe que tinha mais conhecimentos sobre o back-end, tomei a liderança para ajudar meus colegas.
 - Gestão de tempo: como tinha de realizar minhas tasks, ensinar meus colegas a padronização de código e depois revisar o que eles haviam feito, precisei de muita organização.
 - Comunicação: para realizar todas as tarefas, ensinar meus colegas e revisar seus códigos, tive de ter uma comunicação frequente com a equipe.
 
