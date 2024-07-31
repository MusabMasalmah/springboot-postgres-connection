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


## Testing the PostgreSQL Connection

To verify that your Spring Boot application can connect to the PostgreSQL database, follow these steps:

### 1. Open DB Browser for PostgreSQL

1. Launch **DB Browser for PostgreSQL** or any other PostgreSQL database management tool you prefer.

![image](https://github.com/user-attachments/assets/a8da225e-587e-42a8-b916-1551251bd15d)

### 2. Create a New Connection

![image](https://github.com/user-attachments/assets/8d05c37a-71f3-4c8a-8c33-d9f2c14e6e2b)


1. **Add a New Connection:**
   - Click on the option to create a new connection or add a new server. This might be labeled as **"New Connection"**, **"Add Server"**, or something similar, depending on the tool.

2. **Enter Connection Details:**
   - **Host:** `localhost` (or the IP address of your PostgreSQL server)
   - **Port:** `5432` (default port for PostgreSQL)
   - **Database:** `DATABASE_NAME` (replace with your actual database name)
   - **User:** `YOUR_USERNAME` (replace with your actual username)
   - **Password:** `YOUR_PASSWORD` (replace with your actual password)

3. **Test the Connection:**

![image](https://github.com/user-attachments/assets/9a91197c-dcb2-4312-8210-993e6ed22151)

   - Look for a **"Test Connection"** button or similar option. Click it to verify that your application can successfully connect to the PostgreSQL database.
   - If the test is successful, you should see a confirmation message.

4. **Save the Connection:**
   - If the connection test is successful, save the connection settings. You can now use DB Browser to manage and interact with your PostgreSQL database.

### 3. Verify Connection from Spring Boot

Run your Spring Boot application to ensure it can also connect to the PostgreSQL database without errors. Check the application logs for any connection issues.

By following these steps, you can confirm that your PostgreSQL database is properly configured and accessible.

## Conclusion

Thank you for visiting this repository. I hope you find the instructions helpful and that they assist you in setting up and configuring your Spring Boot application with PostgreSQL. 

Wishing you the best of luck with your project and happy coding!

If you have any questions or feedback, feel free to open an issue or reach out. Your contributions and suggestions are always welcome!

Best regards,  
Musab Masalmah

