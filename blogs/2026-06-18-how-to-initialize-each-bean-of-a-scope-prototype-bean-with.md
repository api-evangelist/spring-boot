---
title: "How to initialize each bean of a @Scope(\"prototype\") bean with a different property file?"
url: "https://stackoverflow.com/questions/79962658/how-to-initialize-each-bean-of-a-scopeprototype-bean-with-a-different-prope"
date: "2026-06-18"
author: "Marc Le Bihan"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
I have a Spring Boot ProviderSimulator class that has a @Scope("prototype") , and this value inside: @Service @Scope("prototype") public class ProviderSimulator { @Value("${provider.description}") private String providerDescription; [...] I'm initializing their properties from an application.properties , with this code: @Autowired private ApplicationContext ctx; ProviderSimulator p1 = ctx.getBean(ProviderSimulator.class); ProviderSimulator p2 = ctx.getBean(ProviderSimulator.class); ProviderSimulator p3 = ctx.getBean(ProviderSimulator.class); I have distincts p1 , p2 , p3 beans. But of course, 
