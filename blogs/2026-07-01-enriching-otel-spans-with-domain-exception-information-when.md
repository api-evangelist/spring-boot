---
title: "Enriching OTeL spans with domain exception information when working with Webflux exception handlers"
url: "https://stackoverflow.com/questions/79972120/enriching-otel-spans-with-domain-exception-information-when-working-with-webflux"
date: "2026-07-01"
author: "filpa"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
We have a Spring Webflux-based applications (based on Spring Boot 3.5) that contains a @ControllerAdvice class for centralized exception handling. In our domain services, we have domain-specific exceptions that we map using @ExceptionHandler s, e.g.: @ControllerAdvice public class MyGlobalExceptionHandler { @ExceptionHandler(DomainException.class) public ResponseEntity handleDomainException(DomainException ex) { ... } } This works flawlessly for mapping domain exception to specific error responses containing human readable error codes for our clients, including setting the relevant HTTP respon
