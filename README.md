# Testes de API - Reqres

Este repositório contém testes automatizados para a API Reqres utilizando Postman e Newman. O objetivo é validar o endpoint de criação de usuários da API Reqres.

## Requisitos

- **Node.js**: [Instale o Node.js](https://nodejs.org/) se ainda não o tiver.
- **Newman**: Ferramenta de linha de comando para executar testes Postman.

## Instalação

1. **Clone o Repositório**

   Clone este repositório para o seu ambiente local usando:

   ```bash
   git clone https://github.com/yourusername/yourrepository.git

2. **Instale o Newman**

   ```bash
   git npm install -g newman


## Execução dos Testes

1. **Exporte a Coleção do Postman**

   Certifique-se de que o arquivo de coleção do Postman (Reqres API.postman_collection.json) está localizado no diretório do projeto.


2. **Execute os Testes com o Newman**

   ```bash
   newman run "Reqres API.postman_collection.json"

## Estrutura da Coleção
  
  A coleção Postman inclui os seguintes cenários de teste:
   - Create User - Valid Data: Testa a criação de um usuário com dados válidos.
   - Create User - Missing Name: Testa a criação de um usuário sem o campo "name".
   - Create User - Missing Job: Testa a criação de um usuário sem o campo "job".
   - Create User - Empty Fields: Testa a criação de um usuário com campos vazios.

## Relatórios
  
   **Você pode gerar relatórios detalhados dos testes executados utilizando Newman com a opção -r (reporters). Por exemplo, para gerar um relatório HTML:**

   ```bash
   newman run "Reqres API.postman_collection.json" -r html




