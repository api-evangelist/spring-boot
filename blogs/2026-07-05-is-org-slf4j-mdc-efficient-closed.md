---
title: "is org.slf4j.MDC efficient? [closed]"
url: "https://stackoverflow.com/questions/79974586/is-org-slf4j-mdc-efficient"
date: "2026-07-05"
author: "haoz"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
Is org.slf4j.MDC efficient to store traceId to track process flow? Should I use it in Spring Boot HandlerInterceptor implementationto safely handle hundreds of simultaneous client requests from preHandle to afterCompletion on the production instance? Shoud I use MDC.clear(); in afterCompletion method or MDC.remove(TRACE_ID_NAME);
