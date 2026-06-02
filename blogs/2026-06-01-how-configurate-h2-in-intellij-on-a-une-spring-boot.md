---
title: "how configurate H2 in intellij on a une spring boot application to see tables and sql script execute"
url: "https://stackoverflow.com/questions/79949858/how-configurate-h2-in-intellij-on-a-une-spring-boot-application-to-see-tables-an"
date: "2026-06-01"
author: "flamant"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
i program a small application in spring boot on intellij with H2 data base In my application.properties, I configure the access with H2 spring.jpa.defer-datasource-initialization=true spring.datasource.url=jdbc:h2:file:/data/demo spring.datasource.driverClassName=org.h2.Driver spring.jpa.database-platform=org.hibernate.dialect.H2Dialect spring.datasource.username=sa spring.datasource.password=password spring.sql.init.mode=always At the moment, I have the following error (I work on MAC) Error while creating file "/data" [90062-240] Caused by: java.nio.file.FileSystemException: /data: Read-only 
