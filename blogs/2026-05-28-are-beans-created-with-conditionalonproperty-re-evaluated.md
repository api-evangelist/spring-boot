---
title: "Are beans created with @ConditionalOnProperty re-evaluated after Spring Boot startup?"
url: "https://stackoverflow.com/questions/79948123/are-beans-created-with-conditionalonproperty-re-evaluated-after-spring-boot-sta"
date: "2026-05-28"
author: "J_oslee19"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
I am working on a Spring Boot project where the application can use either MongoDB or PostgreSQL depending on a property value. I have two repository implementations: MongoDB repository: @Repository @ConditionalOnProperty(name = "app.storage", havingValue = "mongo") public class MongoTreeRepository implements TreeRepository { } PostgreSQL repository: @Repository @ConditionalOnProperty(name = "app.storage", havingValue = "postgres") public class PostgresTreeRepository implements TreeRepository { } In application.properties I use either: app.storage=mongo or: app.storage=postgres My service rece
