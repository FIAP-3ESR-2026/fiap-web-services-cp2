# Checkpoint 1 - API de Gerenciamento de Pedidos (Spring Boot)

Este projeto consiste em uma API REST desenvolvida para a avaliação do Checkpoint 1 da FIAP. A aplicação permite realizar o gerenciamento completo de pedidos (CRUD), seguindo as melhores práticas de desenvolvimento com o framework Spring Boot.

## 🚀 Tecnologias Utilizadas

* **Java 21**: Linguagem principal do projeto.
* **Spring Boot 4.0.6**: Framework para construção da API.
* **Spring Data JPA**: Para persistência de dados e mapeamento objeto-relacional.
* **H2 Database**: Banco de dados em memória para ambiente de desenvolvimento.
* **Lombok**: Para redução de código boilerplate (Getters/Setters).
* **Bean Validation**: Para validação dos dados de entrada.
* **Maven**: Ferramenta de gerenciamento de dependências e automação de build.

## 🏗️ Arquitetura do Projeto

A aplicação segue o padrão de arquitetura em camadas para garantir a separação de responsabilidades:

1.  **Model**: Representa a entidade `Pedidos` no banco de dados.
2.  **Repository**: Interface que estende `JpaRepository` para operações de banco de dados.
3.  **Service**: Camada de lógica de negócio da aplicação.
4.  **Controller**: Camada de exposição das rotas (Endpoints) da API.

## 🛠️ Configurações da Aplicação

As configurações de execução e banco de dados estão definidas no arquivo `application.properties`:

* **Porta do Servidor**: 8085.
* **Banco de Dados**: H2 (Arquivo local em `~/testdb`).
* **Console H2**: Disponível em `/h2-console`.
* **Credenciais H2**: Usuário `sa`, Senha `password`.

## 📑 Endpoints da API (Rotas)

A API responde na URL base `http://localhost:8085/orders`.

| Método | Endpoint | Descrição |
| :--- | :--- | :--- |
| **POST** | `/orders` | Cria um novo pedido |
| **GET** | `/orders` | Lista todos os pedidos cadastrados |
| **GET** | `/orders/{id}` | Busca um pedido específico pelo ID |
| **PUT** | `/orders/{id}` | Atualiza os dados de um pedido existente |
| **DELETE** | `/orders/{id}` | Remove um pedido do sistema |

## 📦 Como Executar

1. Clone o repositório.
2. Certifique-se de ter o **JDK 21** instalado.
3. Importe o projeto como um projeto Maven no seu IDE (IntelliJ, Eclipse, etc.).
4. Execute a classe `Checkpoint1Application`.
5. A aplicação estará disponível em `http://localhost:8085`.

---

## 👥 Grupo (Integrantes)

* **Augusto Rocha Silva** - RM556316
* **Erik Yuuta Goto** - RM558076
* **Guilherme Vieira Augusto** - RM557264
* **Wendell dos Santos Silva** - RM558859
