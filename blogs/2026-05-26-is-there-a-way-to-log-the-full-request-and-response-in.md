---
title: "Is there a way to log the full request and response in Spring RestClient on error?"
url: "https://stackoverflow.com/questions/79946629/is-there-a-way-to-log-the-full-request-and-response-in-spring-restclient-on-erro"
date: "2026-05-26"
author: "Aleksander"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
I've been stuck on this task for quite a while. It seems simple, whenever an error happens during a RestClient request, I want to log both the request and response data + body for debugging purposes. However, RestClient only seems to support logging request data.
