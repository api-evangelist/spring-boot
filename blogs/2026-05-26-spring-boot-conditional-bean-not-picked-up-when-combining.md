---
title: "Spring Boot @Conditional bean not picked up when combining @Profile and custom Condition — NoSuchBeanDefinitionException"
url: "https://stackoverflow.com/questions/79946588/spring-boot-conditional-bean-not-picked-up-when-combining-profile-and-custom-c"
date: "2026-05-26"
author: "JHONY ABRAHAM DE LEON PEREZ"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
Problem I'm building a Spring Boot application where a TreeRepository bean must be activated by two conditions simultaneously: a Spring @Profile and a custom @Conditional . The repository is defined like this: java @Repository @Profile("mongo") @Conditional(MongoCondition.class) @Primary public class MongoTreeRepository implements TreeRepository { // ... } MongoCondition reads a property:properties public class MongoCondition implements Condition { @Override public boolean matches(ConditionContext context, AnnotatedTypeMetadata metadata) { String repoType = context.getEnvironment().getProperty
