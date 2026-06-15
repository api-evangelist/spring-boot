---
title: "SpringApplication logger uses mainApplicationClass logger with confusing line numbers"
url: "https://stackoverflow.com/questions/79956101/springapplication-logger-uses-mainapplicationclass-logger-with-confusing-line-nu"
date: "2026-06-10"
author: "Simon Hutchinson"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
c.c.r.r.boot.ReferenceRestApplication:54 - Starting ReferenceRestApplication using Java 25.0.2 with PID 30226 c.c.r.r.boot.ReferenceRestApplication:55 - Running with Spring Boot v4.0.6, Spring v7.0.72026-06-10 08:42:37.251 INFO [main] [reference.boot:refboot-rest:] c.c.r.r.boot.ReferenceRestApplication:658 - The following 2 profiles are active: "local", "personal" The log output shown above is from our application startup. The logs are written by e.g SpringApplication ; however, the mainApplicationClass, ReferenceRestApplication is shown as the logging class, which means that the line number f
