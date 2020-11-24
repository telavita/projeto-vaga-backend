# ACMEVita

Projeto de modelagem de dados e criação de uma API utilizando Python e Flask.

**Este projeto é parte do processo de seleção de desenvolvedor backend da [Telavita](https://telavita.com.br).**

## Sobre o projeto

A ACMEVita está expandindo seus negócios e precisa de um sistema para gerenciar seus departamentos, colaboradores e dependentes.

O seu único desenvolvedor backend está de ferias, você foi recrutado para finalizar este projeto, boa sorte!

### Requisitos

#### Como um Usuário da API eu gostaria de consultar todos os departamentos para visualizar a organização da ACMEVita.

  * Cada departamento deve possuir um *nome do departamento*.
  * A API deve responder com uma listagem de departamentos no formato JSON informando o *nome do departamento* de cada departamento.

#### Como um Usuário da API eu gostaria de consultar todos os colaboradores de um departamento para visualizar a organização da ACMEVita.

  * Cada colaborador deve possuir um *nome completo*.
  * Cada colaborador deve pertencer a *um* departamento.
  * Cada colaborador pode possuir *nenhum, um ou mais* dependententes.
  * A API deve responder com uma listagem de colaboradores do departamento no formato JSON informando o *nome completo* de cada colaborador e a respectiva flag booleana `have_dependents` caso o colaborador possua *um ou mais dependentes*.

### Instruções

1. Faça um _fork_ ou download deste projeto.
2. Trabalhe localmente no seu projeto, faça até o ponto que conseguir.
3. Você está livre para organizar a estrutura do projeto como preferir.
4. Você deve utilizar o Flask para criar os endpoints da API.
4. Você pode utilizar a ORM de sua preferência para modelagem de dados.
5. Suba o seu projeto para o GitLab, GitHub ou qualquer similar.
6. Nos envie o link para o seu projeto, **mesmo que não esteja finalizado!**

**Qualquer dúvida, entre em contato com [Rafael](mailto:rc@telavita.com.br)!**
