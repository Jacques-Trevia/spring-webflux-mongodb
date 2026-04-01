![Java](https://img.shields.io/badge/Java-17-blue.svg)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.x-brightgreen.svg)
![Spring WebFlux](https://img.shields.io/badge/Spring%20WebFlux-Reactive-6DB33F.svg)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?logo=mongodb&logoColor=white)

# ⚡ Spring WebFlux + MongoDB - Backend Reativo
[![NPM](https://img.shields.io/npm/l/react)](https://github.com/Jacques-Trevia/spring-webflux-mongodb/blob/main/LICENSE)

**Spring WebFlux MongoDB** é um projeto backend que implementa uma API REST **reativa** utilizando **Spring WebFlux** e **MongoDB reativo**. O projeto demonstra na prática como construir aplicações não-bloqueantes, escaláveis e de alta performance, aproveitando todo o poder da programação reativa com **Project Reactor**.

* * *

## 🚀 Sobre o Projeto

A aplicação consiste em um sistema de gerenciamento de usuários e posts, explorando os conceitos fundamentais da **programação reativa**:

- Fluxos assíncronos e não-bloqueantes
- Backpressure (controle de fluxo)
- Operadores reativos (`Mono`, `Flux`)
- Integração reativa com MongoDB

* * *

## 🛠️ Tecnologias Utilizadas

| Categoria | Tecnologia |
|-----------|------------|
| **Linguagem** | Java 17 |
| **Framework** | Spring Boot 3.x, Spring WebFlux |
| **Banco de Dados** | MongoDB (Reactive Streams) |
| **Driver Reativo** | Spring Data MongoDB Reactive |
| **Programação Reativa** | Project Reactor (Mono, Flux) |
| **Build** | Maven |

* * *

## 📂 Estrutura do Projeto

O projeto segue a arquitetura de camadas adaptada para o paradigma reativo:

- 📁 **Controllers** – Endpoints da API REST reativa (retornam `Mono`/`Flux`)
- 📁 **Services** – Camada de negócio com operações reativas
- 📁 **Repositories** – Interfaces reativas do Spring Data MongoDB
- 📁 **Models** – Entidades documentadas para MongoDB
- 📁 **DTOs** – Objetos de transferência de dados

* * *

## 📌 Funcionalidades

- ✅ CRUD completo de usuários (criação, consulta, atualização, deleção)
- ✅ CRUD completo de posts associados a usuários
- ✅ Busca paginada e ordenada com suporte reativo
- ✅ Consultas reativas utilizando `Flux` e `Mono`
- ✅ Tratamento de erros com respostas padronizadas
- ✅ Integração com MongoDB reativo (non-blocking)

* * *

## 📦 Como Rodar o Projeto

### 🔧 Pré-requisitos

- [JDK 17](https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html)
- [Maven](https://maven.apache.org/download.cgi)
- [MongoDB](https://www.mongodb.com/try/download/community) (instalado localmente ou via Docker)

### 💾 Banco de Dados

Certifique-se de que o MongoDB esteja em execução:
mongod



### ▶️ Executando a Aplicação

1. Clone o repositório:
git clone https://github.com/Jacques-Trevia/spring-webflux-mongodb.git
cd spring-webflux-mongodb



2. Execute a aplicação com Maven:
mvn spring-boot:run


3. A API estará disponível em **http://localhost:8080**

* * *

## 🔗 Endpoints da API

| Método | Endpoint | Descrição |
|--------|----------|-----------|
| GET | `/users` | Lista todos os usuários (Flux reativo) |
| GET | `/users/{id}` | Busca usuário por ID (Mono reativo) |
| POST | `/users` | Cria um novo usuário |
| PUT | `/users/{id}` | Atualiza um usuário |
| DELETE | `/users/{id}` | Remove um usuário |
| GET | `/users/{id}/posts` | Lista todos os posts de um usuário |
| POST | `/users/{id}/posts` | Adiciona um post a um usuário |

* * *

## 🧪 Testes com Postman

Para facilitar os testes da API, disponibilizo uma coleção do Postman com todas as requisições.

[![Postman](https://img.shields.io/badge/Postman-Collection-FF6C37?logo=postman)](./postman/spring-webflux-collection.json)

* * *

## 🎯 Aprendizados e Desafios

Este projeto foi fundamental para consolidar:

- **Programação Reativa** – Compreensão dos conceitos de `Mono`, `Flux`, backpressure e operadores reativos
- **Spring WebFlux** – Construção de endpoints não-bloqueantes com Router Functions ou anotações
- **MongoDB Reativo** – Utilização do driver reativo e repositórios reativos do Spring Data
- **Escalabilidade** – Entendimento de como aplicações reativas lidam melhor com alta concorrência
- **Arquitetura Assíncrona** – Diferenciação entre modelos síncronos (Spring MVC) e assíncronos (WebFlux)

* * *

## 📜 Licença

Este projeto é parte do curso da **DevSuperior** e tem propósito educacional.

* * *

## 👨‍💻 Autor

**Jacques Araujo Trevia Filho**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/jacques-trevia)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Jacques-Trevia)
