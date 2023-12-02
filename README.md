# parking-control-api 

![Badge Maven Version](https://img.shields.io/badge/maven-v4.0.0-blue)
![Badge Java Version](https://img.shields.io/badge/java-v17-brightgreen)
![Badge Spring Boot Version](https://img.shields.io/badge/spring--boot-v2.7.0-blueviolet)
![Badge Spring Security Version](https://img.shields.io/badge/spring--Security-red)

Este projeto é um sistema de gerenciamento de estacionamento desenvolvido em Java com Spring Boot, utilizando Spring Security para autenticação e autorização, Maven para gerenciamento de dependências, JPA para persistência de dados e PostgreSQL como banco de dados.

## Requisitos

Certifique-se de ter as seguintes ferramentas instaladas em seu ambiente de desenvolvimento:

- Java SDK
- Maven
- PostgreSQL

## Configuração do Banco de Dados

1. Crie um banco de dados no PostgreSQL para o projeto.
2. Atualize as configurações do banco de dados no arquivo `application.properties`.

```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/seu_banco_de_dados
spring.datasource.username=seu_usuario
spring.datasource.password=sua_senha
```
## Autenticação

O projeto utiliza o Spring Security para autenticação. As credenciais padrão são:

- **Usuário:** admin
- **Senha:** senha123

Certifique-se de alterar essas credenciais em um ambiente de produção.

## Endpoints

### Listar Estacionamentos

- **Endpoint:** `/parking-spot?page=0&size=5&sort=registrationDate,ASC)`
- **Método:** GET
- **Descrição:** Retorna uma lista de todos os registros de estacionamentos.

### Detalhes do Estacionamento

- **Endpoint:** `/parking-spot/{id}`
- **Método:** GET
- **Descrição:** Obtém detalhes de um estacionamento específico com base no ID.

### Adicionar Estacionamento

- **Endpoint:** `/parking-spot`
- **Método:** POST
- **Descrição:** Adiciona um novo registro de estacionamento. Envie os dados necessários no corpo da solicitação.

### Excluir Estacionamento

- **Endpoint:** `/parking-spot/{id}`
- **Método:** DELETE
- **Descrição:** Exclui um registro de estacionamento com base no ID fornecido.



#
#
Projeto desenvolvido em aula da professora [Michelli Brito](https://github.com/MichelliBrito).





