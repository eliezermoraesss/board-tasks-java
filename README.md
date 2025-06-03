# 📝 Board Tasks Java

Este é um projeto de portfólio desenvolvido com o objetivo de demonstrar conhecimentos em Java, arquitetura em camadas, acesso a dados (DAO) e versionamento de banco de dados com Liquibase.

## 🚀 Sobre o Projeto

O **Board Tasks Java** é um sistema de gerenciamento de tarefas baseado em camadas, que utiliza o padrão DAO para interagir com o banco de dados. É uma aplicação simples com propósitos educacionais, ideal para demonstrar domínio dos conceitos de persistência, separação de responsabilidades e integração com banco de dados.

### Funcionalidades

- ✅ Criar tarefas
- 📋 Listar tarefas
- ✏️ Atualizar tarefas
- ❌ Remover tarefas
- 📂 Classificação por status

## 🧰 Tecnologias e Ferramentas

- Java 21
- JDBC com padrão DAO
- MySQL
- Liquibase
- Lombok
- Gradle (Kotlin DSL)

## ⚙️ Dependências (Gradle)

```kotlin
plugins {
    id("java")
}

group = "br.com.dio"
version = "1.0-SNAPSHOT"

repositories {
    mavenCentral()
}

dependencies {
    implementation("org.liquibase:liquibase-core:4.29.1")
    implementation("mysql:mysql-connector-java:8.0.33")
    implementation("org.projectlombok:lombok:1.18.34")
    annotationProcessor("org.projectlombok:lombok:1.18.34")
}

tasks.test {
    useJUnitPlatform()
}
```

## 🧪 Como Executar

1. Clone o repositório:
```bash
git clone https://github.com/eliezermoraesss/board-tasks-java.git
cd board-tasks-java
```

2. Configure o banco de dados MySQL e atualize o arquivo de propriedades (`src/main/resources/db.properties` ou similar) com as credenciais corretas.

3. Execute as migrações com o Liquibase (caso esteja configurado via CLI ou integrado ao build).

4. Compile e execute o projeto:
```bash
./gradlew build
java -jar build/libs/board-tasks-java-1.0-SNAPSHOT.jar
```

> Ou execute diretamente pela sua IDE favorita (como IntelliJ IDEA).

## 🗃️ Estrutura de Camadas

- **model**: entidades
- **dao**: acesso ao banco de dados (CRUD)
- **service**: lógica de negócio
- **main**: ponto de entrada da aplicação

## 📌 Observações

- Certifique-se de que o servidor MySQL esteja rodando e acessível.
- Liquibase é usado para versionamento e migração do esquema do banco.
- Lombok simplifica a criação de getters, setters e construtores.

## 🧑‍💻 Autor

Feito com 💙 por [Eliezer Moraes](https://www.linkedin.com/in/eliezer-moraes-silva-80b68010b/)

---

⭐ Se você gostou do projeto, não esqueça de deixar uma estrela no repositório!
