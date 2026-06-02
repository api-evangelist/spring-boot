---
title: "Spring Boot service-level ID counter conflicts with MongoDB persisted documents on application restart"
url: "https://stackoverflow.com/questions/79947216/spring-boot-service-level-id-counter-conflicts-with-mongodb-persisted-documents"
date: "2026-05-27"
author: "JHONY ABRAHAM DE LEON PEREZ"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
Context I have a Spring Boot application with three interchangeable persistence layers: in-memory, PostgreSQL, and MongoDB. The active persistence is chosen via app.storage in application.properties . My TreeService manages node creation with a simple in-memory ID counter: java @Service public class TreeService { private final TreeRepository repo; private final TreeAlgorithmStrategy strategy; private Long idCounter = 1L; public Node createRoot(String value) { Node root = new Node(idCounter++, value, null); return repo.save(root); } public Node addChild(Long parentId, String value) { Node child
