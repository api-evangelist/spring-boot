---
title: "Spring Boot cannot connect to PostgreSQL in Docker"
url: "https://stackoverflow.com/questions/79960757/spring-boot-cannot-connect-to-postgresql-in-docker"
date: "2026-06-16"
author: "SP222"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
I'm having a persistent issue with Spring Boot 3.5.15 connecting to PostgreSQL 16 running in Docker. I keep getting: FATAL: password authentication failed for user "attendance" What I've tried: Docker container runs with correct environment variables: docker run --name postgres -e POSTGRES_USER=attendance -e POSTGRES_PASSWORD=attendance -e POSTGRES_DB=attendance -p 5432:5432 -d postgres:16 I can connect successfully from command line: docker exec -it postgres psql -U attendance -d attendance # Shows: attendance=# User exists in database: SELECT usename FROM pg_user; -- Returns: attendance Envi
