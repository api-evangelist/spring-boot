---
title: "Unable to reproduce SocketReadTimeOut Error for okhttp3"
url: "https://stackoverflow.com/questions/79981310/unable-to-reproduce-socketreadtimeout-error-for-okhttp3"
date: "2026-07-16"
author: "Aditya Mehta"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
We are trying to test ReadTimeOut exception by using useHttps() method of MockWebserver3, but unable to get this error. Please suggest if we can achieve this with useHttps() method, while upgrading springboot from 3.3.x to 3.5.x @Test void shouldThrowSocketTimeoutExceptionOnReadTimeout() { mockWebServer = new MockWebServer(); mockWebServer.useHttps(sslSocketFactory) // Arrange: enqueue a response that delays the body for 5 seconds mockWebServer.enqueue( new MockResponse().Builder .body("This will be delayed") .bodyDelay(5, TimeUnit.SECONDS).inTunnel().build() // Delay sending body ); OkHttpCli
