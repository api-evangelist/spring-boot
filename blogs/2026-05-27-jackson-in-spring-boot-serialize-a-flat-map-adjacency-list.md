---
title: "Jackson in Spring Boot: Serialize a flat Map (adjacency list) into a nested JSON tree without intermediate objects [closed]"
url: "https://stackoverflow.com/questions/79947059/jackson-in-spring-boot-serialize-a-flat-map-adjacency-list-into-a-nested-json"
date: "2026-05-27"
author: "JOSUE RAFAEL PEREZ AGUIRRE"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
I am building a Spring Boot REST API where a strict architectural constraint requires me to implement and expose a tree data structure using only standard Java Collections (e.g., Map, List). I am explicitly forbidden from creating custom Node, Tree, or intermediate DTO classes for this specific engine implementation. The OpenAPI contract expects a deeply nested JSON response, but my tree is maintained in memory as flat maps.
