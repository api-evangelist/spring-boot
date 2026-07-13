---
title: "Spring Boot 3 fails to find bean despite @Service annotation and correct package structure"
url: "https://stackoverflow.com/questions/79978102/spring-boot-3-fails-to-find-bean-despite-service-annotation-and-correct-package"
date: "2026-07-09"
author: "gilson_leonel01"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
I have a Spring Boot 3 application where a controller depends on a service annotated with @Service , but the application fails to start because Spring cannot find the OrderService bean. Error Field orderService in com.mycompany.app.controller.OrderController required a bean of type 'com.mycompany.app.service.OrderService' that could not be found. Project structure src/main/java/com/mycompany/app/ ├── Application.java ├── controller/ │ └── OrderController.java └── service/ └── OrderService.java Application.java package com.mycompany.app; import org.springframework.boot.SpringApplication; import
