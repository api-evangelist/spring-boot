---
title: "Why does Spring Boot not initialize my PostgreSQL data with schema.sql and data.sql?"
url: "https://stackoverflow.com/questions/79946890/why-does-spring-boot-not-initialize-my-postgresql-data-with-schema-sql-and-data"
date: "2026-05-26"
author: "Angello Escobar"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
I am working on a Spring Boot project using PostgreSQL. My goal is to create the tables and insert initial data automatically when the application starts. I have this configuration in my application.properties file: spring.datasource.url=jdbc:postgresql://localhost:5432/progra3db spring.datasource.username=progra3 spring.datasource.password=progra3 spring.datasource.driver-class-name=org.postgresql.Driver spring.sql.init.mode=always spring.jpa.hibernate.ddl-auto=none spring.jpa.show-sql=true spring.jpa.properties.hibernate.format_sql=true My schema.sql file has a table like this: CREATE TABLE 
