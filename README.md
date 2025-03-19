# Gerenciamento de produtos (CRUD-farmacia)

Este é um projeto de Backend para o gerenciamento de farmácia, desenvolvido em Spring Boot. O sistema permite o gerenciamento de produtos farmacêuticos classificados por categoria. O sistema suporta a manipulação de dados de produtos e categorias, oferecendo um CRUD completo para cada um deles. O objetivo principal deste projeto é otimizar o gerenciamento de medicamentos, estoque e organização dos produtos dentro de uma farmácia.

## Tecnologias Usadas

- **Backend**: Java, Spring Boot
- **Banco de Dados**: MySQL
- **Ferramentas**: Maven para gerenciamento de dependências
- **Spring Data JPA**: Para mapeamento objeto-relacional (ORM)
- **Spring Web**: Para implementação das APIs RESTful
- **Spring Boot DevTools**: Para facilitar o desenvolvimento com reinicialização automática
- **IDE**: Spring Boot


## Funcionalidades (CRUD)

Este sistema de farmácia inclui as funcionalidades de CRUD (Create, Read, Update, Delete) para os seguintes recursos:

### Produto

- **Criar Produto (POST)** → `localhost:8080/produtos`
- **Listar Todos os Produtos (GET)** → `localhost:8080/produtos`
- **Buscar Produto por ID (GET)** → `localhost:8080/produtos/{id}`
- **Buscar Produto por Nome (GET)** → `localhost:8080/produtos/nome/{nome}`
- **Atualizar Produto (PUT)** → `localhost:8080/produtos/{id}`
- **Excluir Produto (DELETE)** → `localhost:8080/produtos/{id}`

### Categoria

- **Criar Categoria (POST)** → `localhost:8080/categorias`
- **Listar Todas as Categorias (GET)** → `localhost:8080/categorias`
- **Buscar Categoria por ID (GET)** → `localhost:8080/categorias/{id}`
- **Buscar Categoria por Nome (GET)** → `localhost:8080/categorias/nome/{nome}`
- **Atualizar Categoria (PUT)** → `localhost:8080/categorias/{id}`
- **Excluir Categoria (DELETE)** → `localhost:8080/categorias/{id}`


## Como Rodar o Projeto

1. Clone o repositório para sua máquina local:

    ```bash
    git clone https://github.com/0M1n40/CRUD-Farmacia.git
    ```

2. Navegue até o diretório do projeto:

    ```bash
    cd CRUD-Farmacia
    ```

3. Configure as credenciais do banco de dados em `src/main/resources/application.properties`:

    ```properties
    spring.datasource.url=jdbc:mysql://localhost/db_farmacia?createDatabaseIfNotExist=true&serverTimezone=America/Sao_Paulo&useSSl=false
    spring.datasource.username=usuario
    spring.datasource.password=senha
    ```

4. Execute o projeto com o Maven:

    ```bash
    mvn spring-boot:run
    ```

5. Acesse as APIs RESTful via `http://localhost:8080`.

## Branches

Este projeto utiliza as seguintes branches para controle de versão:

- `configurando-o-Projeto`: Configuração inicial do Spring Boot e do banco de dados.
- `CRUD-Categoria`: Implementação do CRUD completo para o recurso "Categoria".
- `CRUD-produto`: Implementação do CRUD completo para o recurso "Produto".


## Testes

Para validar o funcionamento do sistema, utilize ferramentas como Postman ou Insomnia para realizar chamadas HTTP nas APIs criadas.

Exemplo de requisição para consultar categorias:

```bash
GET http://localhost:8080/categorias
GET http://localhost:8080/produtos

