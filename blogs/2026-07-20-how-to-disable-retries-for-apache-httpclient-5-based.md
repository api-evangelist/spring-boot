---
title: "How to disable retries for Apache HttpClient 5-based RestClient?"
url: "https://stackoverflow.com/questions/79982197/how-to-disable-retries-for-apache-httpclient-5-based-restclient"
date: "2026-07-20"
author: "AlexElin"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
When I have the Apache HttpClient 5 on classpath, then Spring Boot RestClient.Builder bean (from RestClientAutoConfiguration ) produces RestClient s which have retries enabled ( HttpRequestRetryExec from the apache client). How to disable enabling of retries? P.S.
