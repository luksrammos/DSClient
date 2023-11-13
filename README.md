# DSClient - DESAFIO CRUD

Este projeto Java é um sistema de gerenciamento de clientes com operações básicas de CRUD (Create, Read, Update, Delete). Ele utiliza o framework Spring Boot e integra tecnologias como Spring Data JPA para acesso ao banco de dados e Spring Web para criar uma API REST. 

Abaixo estão os principais componentes e funcionalidades do projeto:

## Componentes Principais:

**1. Entidades (entities):**

* A classe Client representa a entidade no banco de dados, mapeada com JPA.

**2. Controladores (controllers):**

* ClientController é um controlador REST que manipula operações relacionadas à entidade Client.

**3. Manipulador de Exceções (handlers):**
* ControllerExceptionHandler: Trata exceções personalizadas e fornece respostas HTTP apropriadas.

**4. DTOs (dto):**
* ClientDTO: Representa a entidade Client de forma simplificada para interações com a API.
* CustomError: DTO para representar erros personalizados.
* ValidationError: Estende CustomError e inclui uma lista de mensagens de erro de campo.

**5. Serviços (services):**
* ClientService: Contém a lógica de negócios para operações relacionadas a clientes.

**6. Exceções (exceptions):**
* DatabaseException: Exceção para erros relacionados a operações no banco de dados.
* ResourceNotFoundException: Exceção para indicar que um recurso não foi encontrado.

**7. Repositórios (repositories):**
* ClientRepository: Interface estendendo JpaRepository para interagir com a entidade Client no banco de dados.

**8. Configurações de Teste (application-test.properties):**
* Configurações específicas para testes usando um banco de dados H2 em memória.

**9. Configurações Gerais (application.properties):**
* Define o perfil ativo como "test".

**10. Dados de Exemplo (import.sql):**
* Contém dados de exemplo para serem importados no banco de dados.

## Funcionalidades Principais:
Operações CRUD: O sistema oferece operações básicas de Create, Read, Update e Delete para entidades Client.
Tratamento de Exceções: Exceções personalizadas são tratadas pelo manipulador de exceções, fornecendo respostas HTTP apropriadas.
Validação de Dados: A validação de dados é realizada usando anotações do Jakarta Validation nos DTOs.

