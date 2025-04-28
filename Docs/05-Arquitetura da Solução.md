# Arquitetura da Solução

**Pré-requisitos**: Consulte o [Projeto de Interface](03-Projeto de Interface.md) para entender as interações que influenciam a estrutura da aplicação.

Este documento descreve a estrutura técnica da solução, incluindo sua arquitetura lógica e física, tecnologias empregadas, estratégia de modelagem de dados e infraestrutura de hospedagem.

![Arquitetura da Solução](img/02-mob-arch.png)

---

## Diagrama de Classes

O diagrama de classes representa graficamente a estrutura interna da aplicação. Ele define as classes que compõem o sistema, seus atributos, métodos e os relacionamentos entre elas. Esse modelo é essencial para compreender como os objetos serão instanciados e como se comunicam durante a execução da aplicação.

> **Referências**:
> - [IBM: Diagramas de Classes](https://www.ibm.com/docs/pt-br/rational-soft-arch/9.6.1?topic=diagrams-class)
> - [Lucidchart: O que é um Diagrama de Classe UML?](https://www.lucidchart.com/pages/pt/o-que-e-diagrama-de-classe-uml)

---

## Modelo Entidade-Relacionamento (ER)

O Modelo ER é utilizado para representar a estrutura lógica dos dados por meio de entidades, atributos e relacionamentos. É a base para a construção do banco de dados e reflete as regras de negócio aplicadas à persistência de dados da aplicação.

> **Referência**:
> - [Lucidchart: Como fazer um diagrama entidade relacionamento](https://www.lucidchart.com/pages/pt/como-fazer-um-diagrama-entidade-relacionamento)

---

## Esquema Relacional

O esquema relacional traduz o Modelo ER em tabelas e colunas com suas respectivas chaves primárias, estrangeiras e restrições de integridade. Este modelo é a base técnica para a implementação do banco de dados relacional.

> **Referência**:
> - [IBM: Criando um modelo relacional](https://www.ibm.com/docs/pt-br/cognos-analytics/10.2.2?topic=designer-creating-relational-model)

---

## Modelo Físico de Banco de Dados

O modelo físico é representado por um arquivo SQL (`banco.sql`) que contém os scripts de criação das tabelas do banco de dados, incluindo índices, restrições e relacionamentos. Esse arquivo deve ser armazenado em `src/bd/`.

---

## Tecnologias Utilizadas

Esta seção lista todas as tecnologias e ferramentas envolvidas no desenvolvimento da solução, incluindo:

- **Linguagens de Programação**: Ex: JavaScript, Python, Dart
- **Frameworks**: Ex: React, Flutter, Django
- **Banco de Dados**: Ex: PostgreSQL, Firebase, SQLite
- **APIs/Serviços Web**: Ex: REST, GraphQL
- **IDE/Editor**: Ex: VSCode, IntelliJ, Android Studio
- **Gerenciadores de Pacotes**: Ex: npm, pip, pub

Também é recomendável incluir um diagrama de alto nível ilustrando como as tecnologias se conectam, por exemplo: do front-end ao back-end, passando por autenticação, banco de dados e serviços externos.

---

## Hospedagem

Descreva a estratégia adotada para publicar a aplicação. Inclua o ambiente escolhido (ex: GitHub Pages, Heroku, Firebase Hosting), motivos para sua escolha, processo de deploy e manutenção contínua.

> **Referências**:
> - [GitHub Pages](https://pages.github.com/)
> - [Repl.it](https://repl.it/)
> - [Heroku](https://devcenter.heroku.com/start)
> - [Publicação no Heroku](http://pythonclub.com.br/publicando-seu-hello-world-no-heroku.html)

---

## Qualidade de Software

Para garantir que o produto atenda às expectativas dos usuários e mantenha padrões técnicos sólidos, a equipe adotou como referência a norma **ISO/IEC 25010**. A norma propõe um modelo com oito características de qualidade, entre elas:

- **Funcionalidade** (adequação, precisão)
- **Usabilidade** (facilidade de uso, acessibilidade)
- **Confiabilidade** (maturidade, disponibilidade)
- **Eficiência** (tempo de resposta, uso de recursos)
- **Manutenibilidade** (modularidade, testabilidade)
- **Portabilidade** (adaptabilidade, instalação)

A equipe selecionou as subcaracterísticas mais relevantes para o contexto do projeto, como:

- **Desempenho**: Monitorado por tempo médio de resposta (métrica: ms por requisição).
- **Confiabilidade**: Validada por testes automatizados e taxa de falhas.
- **Usabilidade**: Avaliada por testes de usabilidade e feedback de usuários.

> **Referências**:
> - [ISO/IEC 25010:2011](https://www.iso.org/standard/35733.html/)
> - [Análise sobre ISO 9126 – NBR 13596](https://www.tiespecialistas.com.br/analise-sobre-iso-9126-nbr-13596/)
> - [Qualidade de Software - DevMedia](https://www.devmedia.com.br/qualidade-de-software-engenharia-de-software-29/18209/)
