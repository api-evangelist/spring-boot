---
title: "Multiple @SpringBootApplication classes in Maven project"
url: "https://stackoverflow.com/questions/79948243/multiple-springbootapplication-classes-in-maven-project"
date: "2026-05-29"
author: "MARIO JOSE BARRERA LINAREZ"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
I'm working on a multi-module Spring Boot project. The application contains two classes annotated with @SpringBootApplication : @SpringBootApplication public class OrganigramaApplication { public static void main(String[] args) { SpringApplication.run(OrganigramaApplication.class, args); } } and @SpringBootApplication public class TreeAppApplication { public static void main(String[] args) { SpringApplication.run(TreeAppApplication.class, args); } } When I execute: mvn spring-boot:run I get the following error: Unable to find a single main class from the following candidates I understand that 
