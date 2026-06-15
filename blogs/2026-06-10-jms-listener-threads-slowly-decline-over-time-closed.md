---
title: "JMS Listener Threads slowly Decline over time [closed]"
url: "https://stackoverflow.com/questions/79956134/jms-listener-threads-slowly-decline-over-time"
date: "2026-06-10"
author: "Frontier"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
I have a Spring Boot Java application using JMSListeners with the DefaultJmsListenerContainerFactory with a maximum concurrency of 300 using AutoAcknowledge . When the application is started, processing proceeds quickly, but begins to tail off after an hour or so. I've added an Aspect over the Listeners that tracks the number of threads in flight and interrupts any thread that's been running for too long.
