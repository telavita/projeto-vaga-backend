# ACMEVita

Projeto de modelagem de dados e criação de uma API utilizando Python e Flask.

**Este projeto é parte do processo de seleção de desenvolvedor backend da [Telavita](https://telavita.com.br).**

## Sobre o projeto

A ACMEVita está expandindo seus negócios e precisa de um sistema para gerenciar seus colaboradores, departamentos, e dependentes.

O seu único desenvolvedor backend está de ferias, você foi recrutado para finalizar este projeto, boa sorte!

### Requisitos

1. Modelagem de dados utilizando a nossa [incrível ORM](docs/IncredibleORM.md):
  * Você está livre para organizar a estrutura de pastas dos modelos como preferir
  * Cada colaborador deve possuir um *ID* e um *nome completo*
  * Cada dependente deve possuir um *ID* e um *nome completo*
  * Cada departamento deve possuir um *ID* e um *nome de departamento*
  * Cada colaborador deve pertencer a **um** departamento
  * Cada colaborador pode possuir **nenhum, um ou mais** dependententes

2. API:
  * Você está livre para organizar a API do jeito que preferir
  * A API deve possuir um endpoint de consulta de todos os departamentos
  * A API deve possuir um endpoint de busca de funcionários e seus respectivos dependentes, por departamento
 
**Não se preocupe se não conseguir atender a todos os requisitos :)**

### Instruções

1. Faça um _fork_ ou download deste projeto.
2. Trabalhe localmente no seu projeto, faça até o ponto que conseguir.
3. Suba o seu projeto para o GitLab, GitHub ou qualquer similar.
4. Nos envie o link para o seu projeto, **mesmo que não esteja finalizado!**

**Qualquer dúvida, entre em contato com [Rafael](mailto:rc@telavita.com.br)!**
