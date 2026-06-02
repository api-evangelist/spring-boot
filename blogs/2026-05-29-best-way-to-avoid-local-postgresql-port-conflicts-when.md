---
title: "Best way to avoid local PostgreSQL port conflicts when using Docker Compose with Spring Boot from Eclipse"
url: "https://stackoverflow.com/questions/79948189/best-way-to-avoid-local-postgresql-port-conflicts-when-using-docker-compose-with"
date: "2026-05-29"
author: "LUIS ANGEL SANTIAGO PALMA"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
I am working on a Spring Boot 3 project that can run with different persistence providers: memory, MongoDB, and PostgreSQL. When I run the whole application with Docker Compose, the Spring Boot container connects to PostgreSQL using the Docker service name: SPRING_DATASOURCE_URL: jdbc:postgresql://postgres:5432/ecommerce That works inside Docker. However, during development we usually run the Spring Boot app from Eclipse and only use Docker for the database.
