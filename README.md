# springboot-postgres-connection

Welcome to Musab Masalmah's GitHub!

This repository demonstrates how to set up a Spring Boot application with PostgreSQL using IntelliJ IDEA. I hope you find this repository helpful and that it benefits you in your development journey.

## Introduction
This project provides a step-by-step guide to integrating Spring Boot with PostgreSQL.

## Prerequisites
- IntelliJ IDEA
- Java 11 or higher
- PostgreSQL

## Setting Up the Project

Go to https://start.spring.io/ , and do the following:

![image](https://github.com/user-attachments/assets/0e2df276-33b1-4c59-95ef-fbbffcc42865)


## Configuring PostgreSQL

To configure PostgreSQL for use with your Spring Boot application, follow these steps:

### 1. Install PostgreSQL
If you haven't already installed PostgreSQL, download and install it from [the PostgreSQL official website](https://www.postgresql.org/download/).

### 2. Create a Database
Once PostgreSQL is installed, you need to create a new database for your application.

![image](https://github.com/user-attachments/assets/c1ae0e89-de68-4968-9825-6b5eada4fb32)


## Configuring PostgreSQL Connection

Go to `src/main/resources/application.properties`

![image](https://github.com/user-attachments/assets/0aecbf20-23c0-4de9-a48f-c63ad3ce2f8c)

and add the following lines:

```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/DATABASE_NAME
spring.datasource.username=YOUR_USERNAME
spring.datasource.password=YOUR_PASSWORD
spring.jpa.hibernate.ddl-auto=create-drop
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.format_sql=true
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.PostgreSQLDialect



