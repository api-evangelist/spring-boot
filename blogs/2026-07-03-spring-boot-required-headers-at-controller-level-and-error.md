---
title: "Spring Boot: Required headers at controller level and error 400 Bad Request instead 404 Not Found"
url: "https://stackoverflow.com/questions/79974168/spring-boot-required-headers-at-controller-level-and-error-400-bad-request-inst"
date: "2026-07-03"
author: "Marcelo"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
I have a @RestController that has a required header. If I specify it in the @RequestMapping annotation family, etc.: @RestController @RequestMapping("/mycontroller", headers = ["X-Custom-Header"]) class MyController { @GetMapping fun hello() = "Hello World" } If the user doesn't send it, a 404 Not Found error is generated with the message No static resource mycontroller. However, if I specify it as a parameter of the method: @RestController @RequestMapping("/mycontroller") class MyController { @GetMapping fun hello( @RequestHeader("X-Custom-Header") header: String, ) = "Hello World" } If the u
