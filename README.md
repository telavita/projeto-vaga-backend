# ACMEVita - Corporação de saúde mental

Projeto de modelagem de dados e criação de uma API utilizando Python e Flask.

**Este projeto é parte do processo de seleção de desenvolvedor backend da [Telavita](https://telavita.com.br).**

## Sobre o projeto

A ACMEVita está expandindo seus negócios e precisa de um sistema para gerenciar seus colaboradores, departamentos, e dependentes.

O seu único desenvolvedor backend está de ferias, então você foi recrutado para este projeto, boa sorte!

### Requisitos

1. Modelagem de dados utilizando a nossa incrível ORM (documentada abaixo):
  * Você está livre para organizar a estrutura de pastas dos modelos como preferir
  * Cada colaborador deve pertencer a **um** departamento
  * Cada departamento deve possuir um *ID* e um *nome de departamento*
  * Cada colaborador pode possuir **nenhum, um ou mais** dependententes
  * Cada dependent  e deve possuir um *ID* e um *nome completo*
  * Cada funcionário deve possuir um *ID* e um *nome completo*

2. API e seus endpoints:
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

---

# IncredibleORM: Nossa incrível ORM

Essa é a ORM mais avançada do mercado e você vai utiliza-la para modelar seus dados.

## Declarando um modelo

```
class MyModel(IncredibleModel):
    field = IncredibleField(arg=value)

    def my_method(self):
        return something
```

## Tipos de campos

### IncredibleIntegerField

Este tipo de campo representa um número inteiro e utiliza o tipo de dados `int` do Python.

Args:
- `optional`: Indica se o campo é obrigatório (o padrão é `True`)

Exemplo:
> IncredibleIntegerField(optional=False)

### IncredibleCharField

Este tipo de dados representa uma sequência de caracteres e utiliza o tipo `string` do Python.

Args:
- `optional`: Indica se o campo é obrigatório (o padrão é `True`)
- `max_length`: Tamanho máximo da sequência de caracteres (requerido)

Exemplo:
> IncredibleCharField(optional=False, max_length=20)

### IncredibleForeignKey    

Este tipo de dados representa uma relação entre dois modelos.

Args:
- `optional`: Indica se o campo é obrigatório (o padrão é `True`)
- `to`: Modelo alvo da relação

Exemplo:
> IncredibleForeignKey(optional=False, to=AnotherModel)

