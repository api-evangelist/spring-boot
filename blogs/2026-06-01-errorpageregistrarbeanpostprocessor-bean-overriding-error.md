---
title: "ErrorPageRegistrarBeanPostProcessor bean overriding error"
url: "https://stackoverflow.com/questions/79949458/errorpageregistrarbeanpostprocessor-bean-overriding-error"
date: "2026-06-01"
author: "PEREZ MONSIVAIS JOSE DE JESUS"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
I created a MyApplication.java file following the tutorial under the URL linked below using maven. https://docs.spring.io/spring-boot/tutorial/first-application/index.html import org.springframework.boot.SpringApplication; import org.springframework.boot.autoconfigure.SpringBootApplication; import org.springframework.web.bind.annotation.RequestMapping; import org.springframework.web.bind.annotation.RestController; @RestController @SpringBootApplication public class MyApplication { @RequestMapping("/") String home() { return "Hello World!"; } public static void main(String[] args) { SpringAppli
