---
title: "\"Cannot set the Security Context\" console message"
url: "https://stackoverflow.com/questions/79960817/cannot-set-the-security-context-console-message"
date: "2026-06-16"
author: "haoz"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
During obtaining the authentication token the following message appears in the Spring Boot application console. Cannot set the Security Context I think it's important that this message doesn't include any Java class path, date, or time, as if its source wasn't a logger used in a Spring Boot application. To obtain the token, I use the following methods in the controller and service: @RequiredArgsConstructor @RestController @CrossOrigin @DependsOn({JwtPublicAuthenticationService.BEAN_NAME}) public class JwtPublicAuthenticationController { private final JwtPublicAuthenticationService jwtPublicAut
