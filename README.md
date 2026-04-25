# Checkpoint 1 - API de Gerenciamento de Pedidos (Spring Boot)

Este projeto consiste em uma API REST desenvolvida para a avaliação do Checkpoint 1 da FIAP. [cite_start]A aplicação permite realizar o gerenciamento completo de pedidos (CRUD), seguindo as melhores práticas de desenvolvimento com o framework Spring Boot[cite: 1, 2].

## 🚀 Tecnologias Utilizadas

* [cite_start]**Java 21**: Linguagem principal do projeto[cite: 2].
* [cite_start]**Spring Boot 4.0.6**: Framework para construção da API[cite: 2].
* [cite_start]**Spring Data JPA**: Para persistência de dados e mapeamento objeto-relacional[cite: 2].
* [cite_start]**H2 Database**: Banco de dados em memória para ambiente de desenvolvimento[cite: 2].
* [cite_start]**Lombok**: Para redução de código boilerplate (Getters/Setters)[cite: 2].
* [cite_start]**Bean Validation**: Para validação dos dados de entrada[cite: 2].
* [cite_start]**Maven**: Ferramenta de gerenciamento de dependências e automação de build[cite: 2].

## 🏗️ Arquitetura do Projeto

A aplicação segue o padrão de arquitetura em camadas para garantir a separação de responsabilidades:

1.  [cite_start]**Model**: Representa a entidade `Pedidos` no banco de dados[cite: 6, 13].
2.  [cite_start]**Repository**: Interface que estende `JpaRepository` para operações de banco de dados[cite: 34, 35].
3.  [cite_start]**Service**: Camada de lógica de negócio da aplicação[cite: 37, 52].
4.  [cite_start]**Controller**: Camada de exposição das rotas (Endpoints) da API[cite: 56, 58].

## 🛠️ Configurações da Aplicação

[cite_start]As configurações de execução e banco de dados estão definidas no arquivo `application.properties`[cite: 95]:

* [cite_start]**Porta do Servidor**: 8085[cite: 98].
* [cite_start]**Banco de Dados**: H2 (Arquivo local em `~/testdb`)[cite: 100].
* [cite_start]**Console H2**: Disponível em `/h2-console`[cite: 108].
* [cite_start]**Credenciais H2**: Usuário `sa`, Senha `password`[cite: 100].

## 📑 Endpoints da API (Rotas)

[cite_start]A API responde na URL base `http://localhost:8085/orders`[cite: 60, 98].

| Método | Endpoint | Descrição |
| :--- | :--- | :--- |
| **POST** | `/orders` | [cite_start]Cria um novo pedido [cite: 65, 70] |
| **GET** | `/orders` | [cite_start]Lista todos os pedidos cadastrados [cite: 72, 73] |
| **GET** | `/orders/{id}` | [cite_start]Busca um pedido específico pelo ID [cite: 75, 79] |
| **PUT** | `/orders/{id}` | [cite_start]Atualiza os dados de um pedido existente [cite: 81, 86] |
| **DELETE** | `/orders/{id}` | [cite_start]Remove um pedido do sistema [cite: 88, 92] |

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
