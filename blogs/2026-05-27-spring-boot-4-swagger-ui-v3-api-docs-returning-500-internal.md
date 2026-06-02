---
title: "Spring Boot 4, Swagger UI, /v3/api-docs returning 500 Internal Server Error with NO backend logs [closed]"
url: "https://stackoverflow.com/questions/79947170/spring-boot-4-swagger-ui-v3-api-docs-returning-500-internal-server-error-with"
date: "2026-05-27"
author: "M. Fahman"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
I'm running into a completely silent 500 error with SpringDoc OpenAPI and could really use some pointers. My Stack: Spring Boot 4.0.5 Java 21 SpringDoc OpenAPI Starter WebMVC UI 2.6.0 Maven The Issue: When I boot up the application, it starts successfully on port 8080. However, when I navigate to http://localhost:8080/swagger-ui/index.html , the UI loads but immediately throws a "Failed to load API definition" popup.
