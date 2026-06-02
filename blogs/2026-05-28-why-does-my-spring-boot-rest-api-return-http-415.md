---
title: "Why does my Spring Boot REST API return HTTP 415 Unsupported Media Type when sending JSON from Postman?"
url: "https://stackoverflow.com/questions/79948084/why-does-my-spring-boot-rest-api-return-http-415-unsupported-media-type-when-sen"
date: "2026-05-28"
author: "J_oslee19"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
I am learning how REST APIs work in Spring Boot and found an issue when sending JSON data to a controller endpoint. My API returns: HTTP 415 Unsupported Media Type even though the JSON body itself seems valid. Controller example: @RestController @RequestMapping("/users") public class UserController { @PostMapping public String createUser(@RequestBody User user) { return "User created"; } } Model: public class User { private String name; private int age; public String getName() { return name; } public void setName(String name) { this.name = name; } public int getAge() { return age; } public voi
