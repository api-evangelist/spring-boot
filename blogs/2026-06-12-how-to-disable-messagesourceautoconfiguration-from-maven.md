---
title: "How to disable MessageSourceAutoConfiguration from maven parent"
url: "https://stackoverflow.com/questions/79956991/how-to-disable-messagesourceautoconfiguration-from-maven-parent"
date: "2026-06-12"
author: "Dario Viva"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
We have some special requirements on how we need to use our message source. Thats why we have autoconfigured our own message source configuration beans. In Spring Boot 3 this worked just fine, we did not even need to exclude the MessageSourceAutoConfiguration bean.
