# java-back-end

Este repositório contém o código do projeto Java Back End.

## Serviços

A aplicação é composta de três microserviços, a user-api, a product-api e a shopping-api.

A user-api possui os serviços para gerenciar os usuários da aplicação.

A product-api possui os serviços para gerenciar os produtos disponíveis para compras.

A shopping-api os serviços para que usuários realizem compras.

## Banco de dados

As aplicações criam as tabelas automaticamente quando são executadas pela primeira vez, porém o banco de dados deve ser criado no postgres.

As aplicações estão configuradas para se conectar ao banco de dados `dev`, por isso antes de rodar as aplicações, crie esse banco de dados. Se quiser alterar o nome do banco de dados, altere o arquivo application.properties de cada projeto. Utilizando o docker compose, esse banco de dados já é criado automaticamente.

Todos os projetos acessam o mesmo banco de dados, apenas criam schemas diferentes.

## Postman

o arquivo `livro-back-end-java.postman_collection.json` é uma collection do Postman que possui as chamadas para os serviços da aplicação. A collection está configurada para chamar os serviços já no Kubernetes. Para chamar na execução local, basta trocar o shopping.com para localhost:808x.

## Execução

A maneira mais simples de executar a aplicação é utilizando o docker-compose, para isto, basta executar o comando `docker-compose up` depois que a imagem docker dos microserviços forem criadas.

## Versões

As aplicações foram desenvolvidas com a versão 3.0.0 do Spring Boot e o Java 17.
# Java Back End

Este repositório contém o código do livro Java Back End.

## 🚀 Tecnologias Utilizadas

![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=java&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=for-the-badge&logo=spring-boot&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)

## 📑 Serviços

A aplicação é composta de três microserviços: `user-api`, `product-api` e `shopping-api`.

- `user-api`: Gerencia os usuários da aplicação.
- `product-api`: Gerencia os produtos disponíveis para compras.
- `shopping-api`: Permite que usuários realizem compras.

## 🛢 Banco de Dados

As tabelas são criadas automaticamente na primeira execução, mas é necessário criar o banco de dados no PostgreSQL previamente.

- Banco de dados: `dev`
- Docker Compose: Cria o banco automaticamente.
- Os projetos compartilham o mesmo banco de dados, com schemas separados.

## 📬 Postman

O arquivo `livro-back-end-java.postman_collection.json` contém uma collection do Postman com chamadas para os serviços da aplicação. 

- Configurado para Kubernetes, mas adaptável para execução local.

## 🛠 Execução

A maneira mais simples de executar a aplicação é utilizando o Docker Compose:

```bash
docker-compose up
