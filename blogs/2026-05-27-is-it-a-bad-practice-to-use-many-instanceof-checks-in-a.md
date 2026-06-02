---
title: "Is it a bad practice to use many instanceof checks in a Spring Boot REST controller to map multiple persistence models?"
url: "https://stackoverflow.com/questions/79947506/is-it-a-bad-practice-to-use-many-instanceof-checks-in-a-spring-boot-rest-control"
date: "2026-05-27"
author: "LESTER PAYES"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
I am building a Spring Boot REST API for a tree structure. The project uses an OpenAPI contract-first approach, so my controller implements a generated interface: java @RestController public class TreeController implements TreeApi{ The API must support multiple storage implementations selected by configuration: app.storage=memory app.storage=postgres app.storage=mongo The response models come from OpenAPI, for example: NodeResponse TreeNodeResponse NodeListResponse NumberResponse ValidationResponse The problem is that each storage implementation returns a different internal model: CustomTreeNo
