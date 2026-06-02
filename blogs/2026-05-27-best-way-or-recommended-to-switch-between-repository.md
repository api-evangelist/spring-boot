---
title: "Best way or recommended to switch between repository implementations in Spring Boot without manually editing application.properties?"
url: "https://stackoverflow.com/questions/79947614/best-way-or-recommended-to-switch-between-repository-implementations-in-spring-b"
date: "2026-05-27"
author: "Alejandro Campos"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
I am working on a Spring Boot project where I have multiple repository implementations for the same interface. For example: an in-memory implementation a PostgreSQL implementation a MongoDB implementation I also have different tree-processing strategies in the application depending on configuration. Currently I switch implementations manually using a property in application.properties : app.storage=memory and then use @ConditionalOnProperty : @Repository @ConditionalOnProperty( name = "app.storage", havingValue = "memory" ) public class MemoryTreeRepository implements TreeRepository { } This w
