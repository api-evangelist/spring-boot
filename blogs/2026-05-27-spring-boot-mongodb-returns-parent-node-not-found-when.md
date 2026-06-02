---
title: "Spring Boot MongoDB returns \"Parent node not found\" when creating child nodes in tree structure [duplicate]"
url: "https://stackoverflow.com/questions/79947162/spring-boot-mongodb-returns-parent-node-not-found-when-creating-child-nodes-in"
date: "2026-05-27"
author: "LESTER PAYES"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
I am building a Spring Boot API for a tree structure that supports multiple storage implementations (memory, PostgreSQL and MongoDB ). The storage implementation is selected using properties like: properties app.storage=postgres or: app.storage=mongo API Endpoint The endpoint for creating child nodes is: POST /nodes/{parentId}/children The controller receives the parent ID as Long : @Override public NodeResponse nodesParentIdChildrenPost(Long parentId, NodeRequest nodeRequest) { Object child = persistenceService.addChild(parentId, nodeRequest.getName()); return toNodeResponse(child); } Postgre
