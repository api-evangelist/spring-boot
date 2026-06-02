---
title: "Spring Boot @ConditionalOnProperty bean not activating with CLI arguments"
url: "https://stackoverflow.com/questions/79949126/spring-boot-conditionalonproperty-bean-not-activating-with-cli-arguments"
date: "2026-05-31"
author: "Héctor Mellado"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
Problem I have a Spring Boot 3 multimodule project where I use @ConditionalOnProperty to switch between persistence strategies (H2, PostgreSQL, MongoDB) at runtime. The bean is not being activated when I pass the property via --app.persistence.type=mongo as a command line argument. Configuration application.properties (only base config, no persistence type defined here): spring.application.name=app server.port=8080 Bean configuration: @Configuration public class PersistenceConfig { @Bean @ConditionalOnProperty(name = "app.persistence.type", havingValue = "mongo") public PersistenceStrategy mon
