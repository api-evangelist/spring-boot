---
title: "Spring Boot fails to start: Port 8080 already in use, taskkill access denied on Windows [closed]"
url: "https://stackoverflow.com/questions/79947117/spring-boot-fails-to-start-port-8080-already-in-use-taskkill-access-denied-on"
date: "2026-05-27"
author: "Josue Paniagua"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
I am trying to run my Spring Boot application on Windows but it fails with this error: Web server failed to start. Port 8080 was already in use. I tried to find the process using the port: netstat -ano | findstr :8080 Result: TCP 0.0.0.0:8080 0.0.0.0:0 LISTENING 8580 Then I tried to kill the process: taskkill /PID 8580 /F But got: Error: Access is denied.
