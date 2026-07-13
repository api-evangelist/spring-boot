---
title: "How to set a default request body value"
url: "https://stackoverflow.com/questions/79979675/how-to-set-a-default-request-body-value"
date: "2026-07-10"
author: "Lako12"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
I upgraded my application from Spring Boot 3 to Spring Boot 4, so I also updated Jackson. However, I encountered a problem. If I have an endpoint that takes an object like @RequestBody , and I define an attribute like this inside it: private boolean required = true; The default value of true is ignored, while this wasn't the case with Jackson 2.
