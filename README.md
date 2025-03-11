# study-apiw

![Java](https://img.shields.io/badge/Java-17-blue) ![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.4.3-green) ![Maven](https://img.shields.io/badge/Maven-4.0.0-orange)

## 📌 Sobre o Projeto

O **study-apiw** é uma aplicação de estudo desenvolvida com **Java 17** e **Spring Boot 3.4.3**, com o objetivo de explorar conceitos básicos de APIs REST. Este projeto faz parte do material de estudo da aula **"Arquitetura Orientada a Serviços (SOA) e Web Services"**.

## 🚀 Tecnologias Utilizadas

- **Java 17**
- **Spring Boot 3.4.3**
- **Spring Web**
- **SpringDoc OpenAPI** (Swagger UI)
- **Maven**

## 📁 Estrutura do Projeto

```
study-apiw/
├── src/
│   ├── main/
│   │   ├── java/com/github/akiozin/study_apiw/
│   │   │   ├── StudyApiwApplication.java
│   │   │   ├── ControllerPing.java
│   │   │   ├── ControllerProduto.java
│   │   │   ├── Produto.java
│   │   └── resources/application.properties
│   └── test/
├── pom.xml
├── README.md
```

## 📡 Endpoints Disponíveis

### 🔹 Teste de Conectividade

`GET /ping` → Retorna `pong` para verificar se a API está funcionando corretamente.

### 🔹 Gerenciamento de Produtos

| Método  | Endpoint    | Descrição |
|----------|------------|-------------|
| `POST`   | `/produtos` | Cria um novo produto (retorna uma mensagem fixa). |
| `PUT`    | `/produtos` | Atualiza um produto (retorna uma mensagem fixa). |
| `GET`    | `/produtos` | Retorna um produto (mensagem fixa `"Maça"`). |
| `DELETE` | `/produtos` | Exclui um produto e retorna `204 No Content`. |

## 🛠️ Como Executar o Projeto

### 🔹 Requisitos

- Java 17+
- Maven 4.0.0+

### 🔹 Passos

1. **Clone o repositório:**
   ```sh
   git clone https://github.com/Akiozin/study-apiw.git
   ```
2. **Acesse o diretório:**
   ```sh
   cd study-apiw
   ```
3. **Compile e execute o projeto:**
   ```sh
   ./mvnw spring-boot:run  # Linux/macOS
   mvnw.cmd spring-boot:run # Windows
   ```
4. **Acesse a API via browser ou ferramenta como Postman:**
   ```
   http://localhost:8080/ping
   ```

## 📄 Licença

Este projeto está sob a licença MIT - consulte o arquivo [LICENSE](LICENSE) para mais detalhes.
