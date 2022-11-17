#  JOBNATION

## Introdução

A parceiria da FATEC junto a empresa JET SOFT, porpocionou aos alunos do 4° semestre do curso de Banco de Dados, o desafio onde eles deveriam apresentar uma solução tecnológica para sanar e atender às necessidades do mesmo. 
    
## Proposta:
Desenvolver uma API que possibilita a busca de candidatos a partir de uma vaga, buscando uma contratação veloz e assertiva. Dentre os critérios, deverão ser destaques a segurança e o desempenho da aplicação.

Esta API deve realizar a busca por localização: número de conduções para chegar ao local de trabalho; busca por diferentes critérios: rota(s) de pesquisa estão sendo desenhadas para propiciar liberdade de consulta ao BD. Nesse passo, a aplicação varrerá currículos já cadastrados e identificará candidato(s) mais adequados à vaga.

Diagrama de caso de uso:
<details>
  <summary>Clique aqui para visualizar o Padrão de Projeto Proxy</summary>
  <br>
   <img style="border-radius: 50%;" src="https://github.com/GabrielSG20/Portfolio/blob/main/images/Model-1.png](https://user-images.githubusercontent.com/61089745/159176256-013d0b24-b377-4d74-a132-cef3b569b13c.png" width="800px;" alt=""/>
  </details>

## Tecnologias

- Oracle 11g (Sql developer): É um banco de dados popular e relacional, foi usado para criar PROCEDURE PL/SQL: Consulta de candidatos por distância (LAT,LONG); PROCEDURE  de devolução de listas por Múltiplos  Critérios com CURSOR; População do BD com dados fictícios para teste de PERFORMANCE;

- Java (IntelliJ / Eclipse): Java é uma linguagem de programação orientada a objetos, para desenvolver o backend foi usado os ambientes Eclipse e Intellij para desenvolvimento integrado, escrito em Java. 

- Javascript (Node-JS): JavaScript é uma linguagem de programação interpretada estruturada, de script em alto nível. Foi utilizada essa linguagem para fazer a aplicação consumir os dados da API do Google Maps.

- Insomnia/POSTMAN: É uma API Client que facilita aos desenvolvedores criar, compartilhar, testar e documentar APIs. Usamos essas API's para testar o backend com as requisições GET, POST, PUT, DELETE e o match entre os candidatos e vagas.

- GitLab: Gerenciador de repositório de software baseado em git, com suporte a Wiki, gerenciamento de tarefas e CI/CD. Guardamos o código do projeto nesse repositório.

- OBS Studio / Kdenlive: É um programa de streaming e gravação gratuito. Foi gravado as telas da aplicação e apresentação usando a ferramenta OBS Studio.

- API Google Maps: É um serviço público e gratuito que qualquer pessoa pode usar em seus sites e aplicações. A API foi usada para buscar quantidade de meios de transporte necessárias ao candidato chegar ao local de trabalho.

## Contribuições individuais 

Nesse projeto como o foco era o backend e banco de dados não era um requisito ter frontend na aplicação, portanto nas divisões de tasks na equipe escolhi contribuir como de costume a aplicação, ajudando a desenvolver o backend.

Sendo a integrante do grupo com mais conhecimento em Java juntod da framework Spring, dei inicio ao projeto e ensinei aos colegas a desenvolver o mesmo. Com isso, demostrei como utilizo 9 camadas para desenvolvimento das entidades das quais foram definidas.

![image](https://user-images.githubusercontent.com/61089745/164765729-75257564-823f-4901-8cb2-55be55c0759c.png)

 O metodo que eu utilizo chama (MPConConRVS) Model, Payload, Converter, Repository, Validator, Services, Controller.

Fiquei responsável por criar as respectivas camadas e revisar as que meus colegas fizeram.

![image](https://user-images.githubusercontent.com/61089745/164775826-1cccd9f0-f193-4cd6-b864-38682c7a4365.png)

## Aprendizados efetivos

### Hard Skills 

- Neste semestre eu aperfeiçoei meus conhecimentos em Java.

### Soft Skills
 - Gestão de tempo
 - Liderança do back-end;
 - Autonomia.
