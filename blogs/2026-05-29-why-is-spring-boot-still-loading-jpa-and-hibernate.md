---
title: "Why is Spring Boot still loading JPA and Hibernate configuration when using another active profile?"
url: "https://stackoverflow.com/questions/79948309/why-is-spring-boot-still-loading-jpa-and-hibernate-configuration-when-using-anot"
date: "2026-05-29"
author: "JEINER ANDY JOSUE PINEDA CORLE"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
I am working on a Spring Boot project with multiple profiles. I currently have profiles such as: application.properties application-memory.properties application-mongo.properties The idea is that each profile should load different configurations depending on the storage implementation being used. However, I noticed that even when I activate another profile like "memory", Spring Boot still tries to initialize JPA and Hibernate automatically.
