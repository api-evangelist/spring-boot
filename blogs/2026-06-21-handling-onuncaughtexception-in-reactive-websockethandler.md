---
title: "Handling onUncaughtException in Reactive WebSocketHandler Spring Boot 3"
url: "https://stackoverflow.com/questions/79964795/handling-onuncaughtexception-in-reactive-websockethandler-spring-boot-3"
date: "2026-06-21"
author: "lafual"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
Given the following snippet of code @Component("myWebSocketHandler") public class MyWebSocketHandler implements WebSocketHandler { @Override public Mono handle(WebSocketSession session) { return session .send( myFluxSource .doOnError(System.err::println) .onErrorResume(e -> Mono.empty()) .map(p -> p.toString()) ) .doOnError(System.err::println) .onErrorResume(e -> Mono.empty()) } If I interrupt the TCP connection, in order to simulate a comms issue between the client (Javascript WebSocket) and the Spring Boot Reactive server, I get the following stack trace (I replaced IPs with xxx yyy) 2026-0
