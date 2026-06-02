---
title: "Spring Boot does not create a bean with @ConditionalOnProperty even though the property exists"
url: "https://stackoverflow.com/questions/79948112/spring-boot-does-not-create-a-bean-with-conditionalonproperty-even-though-the-p"
date: "2026-05-28"
author: "LUIS ANGEL SANTIAGO PALMA"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
I am working on a Spring Boot 3 application with Java 17. The app can switch the tree algorithm strategy using a property from application.properties . My application.properties file contains: app.storage=memory app.tree-strategy=custom server.port=8080 This is my configuration class: @Configuration public class TreeStrategyConfig { @Bean @ConditionalOnProperty(name = "app.tree-strategy", havingValue = "custom", matchIfMissing = true) public TreeAlgorithmStrategy customTreeStrategy() { return new CustomTreeImpl(); } @Bean @ConditionalOnProperty(name = "app.tree-strategy", havingValue = "collec
