# Arquitetura da Solução

> **Pré-requisito:** Consulte o documento <a href="04-Projeto de Interface.md"> Projeto de Interface </a> para melhor compreensão da integração visual com a arquitetura da aplicação.

Este documento descreve a estrutura da solução em termos de componentes principais, modelagem de dados, tecnologias envolvidas e ambiente de hospedagem.

![Arquitetura da Solução](img/02-mob-arch.png)

---

## Diagrama de Classes

O diagrama de classes define a estrutura estática do sistema, especificando as classes que compõem a aplicação, seus atributos, métodos e os relacionamentos entre elas. Ele serve como base para a implementação orientada a objetos e para a definição de responsabilidades de cada componente no sistema.

---

## Modelo Entidade-Relacionamento (ER)

O modelo ER descreve conceitualmente os dados manipulados pela aplicação, representando as entidades do domínio e seus relacionamentos. Ele é essencial para garantir a integridade lógica da base de dados e para facilitar a comunicação entre desenvolvedores e analistas.

---

## Esquema Relacional

Tradução do Modelo ER para o modelo lógico, o esquema relacional organiza os dados em tabelas e define as chaves primárias, estrangeiras e restrições de integridade. Esse artefato é crucial para a implementação do banco de dados relacional.

---

## Modelo Físico

Deve ser entregue um arquivo `banco.sql` contendo os scripts SQL necessários para a criação das estruturas do banco de dados. Este arquivo deve ser incluído na pasta `src/bd`.

---

## Tecnologias Utilizadas

Liste aqui todas as tecnologias adotadas na implementação da solução, como linguagens de programação, frameworks, bibliotecas, IDEs, serviços web, entre outros.

Adicionalmente, inclua um diagrama ou fluxograma que ilustre o fluxo de interação do usuário com o sistema e como os componentes tecnológicos estão integrados, desde a entrada até o retorno da resposta.

---

## Hospedagem

Descreva o ambiente de hospedagem escolhido para disponibilizar a aplicação (e.g., Heroku, GitHub Pages, Repl.it), bem como o processo de publicação e atualização da plataforma.

---

## Qualidade de Software

A qualidade de software é um fator crítico no desenvolvimento e entrega de soluções robustas, manuteníveis e escaláveis. A norma ISO/IEC 25010 define oito características principais de qualidade e suas subcaracterísticas.

Sua equipe deve selecionar as subcaracterísticas mais relevantes para o projeto e justificar a escolha com base nos objetivos do sistema e nas necessidades dos usuários. Também é importante definir métricas que permitam avaliar essas qualidades ao longo do desenvolvimento.
