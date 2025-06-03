# 📝 Board Tasks Java

Este é um projeto de portfólio desenvolvido com o objetivo de demonstrar habilidades em Java, Spring Boot e boas práticas de desenvolvimento de APIs REST.

## 🚀 Sobre o Projeto

O **Board Tasks Java** é uma API para gerenciamento de tarefas (Kanban), onde é possível criar, listar, atualizar e excluir tarefas.

### Funcionalidades

- ✅ Criar tarefas
- 📋 Listar todas as tarefas
- ✏️ Atualizar informações de uma tarefa
- ❌ Remover tarefas
- 📂 Organizar tarefas por status (To Do, Doing, Done)

## 🛠️ Tecnologias Utilizadas

- Java 21
- Spring Boot 3.4.3
- Gradle (com Kotlin DSL)
- Spring Web
- Spring Data JPA
- PostgreSQL (ou H2 para testes)
- Swagger / OpenAPI
- Lombok
- Docker (opcional)
- Testes com JUnit e Mockito

## 📁 Estrutura do Projeto

```
src
├── main
│   ├── java
│   │   └── com.eliezer.boardtasks
│   └── resources
│       └── application.properties
└── test
    └── java
        └── com.eliezer.boardtasks
```

## 🧪 Como Executar

1. Clone o repositório:
```bash
git clone https://github.com/eliezermoraesss/board-tasks-java.git
cd board-tasks-java
```

2. Execute o projeto com Gradle Wrapper:
```bash
./gradlew bootRun
```

3. Acesse o Swagger para explorar os endpoints:
```
http://localhost:8080/swagger-ui.html
```

## 📌 Observações

- Certifique-se de ter o Java 21 instalado na sua máquina.
- O banco de dados pode ser configurado no arquivo `application.properties` ou via variáveis de ambiente.

## 🧑‍💻 Autor

Feito com 💙 por [Eliezer Moraes](https://www.linkedin.com/in/eliezer-moraes-silva-80b68010b/)

---

⭐ Se você gostou do projeto, não esqueça de deixar uma estrela no repositório!