---
title: "Maven clean fails with AccessDeniedException while compile succeeds on Windows 11"
url: "https://stackoverflow.com/questions/79979896/maven-clean-fails-with-accessdeniedexception-while-compile-succeeds-on-windows-1"
date: "2026-07-11"
author: "Niranjan"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
I'm facing an unusual issue with Maven where `compile` works successfully, but `clean` always fails with an `AccessDeniedException`. ## Environment - Windows 11 - Oracle JDK 26.0.1 - Apache Maven 3.9.16 (Maven Wrapper) - Spring Boot 4.1.0 - IntelliJ IDEA Community Edition ## Java and Maven versions ```text java -version java version "26.0.1" ``` ```text .\mvnw.cmd -version Apache Maven 3.9.16 Java version: 26.0.1 Java home: C:\Program Files\Java\jdk-26.0.1 ``` ## Compile succeeds ```bash .\mvnw.cmd compile ``` Output: ```text [INFO] BUILD SUCCESS ``` ## Clean fails ```bash .\mvnw.cmd clean ```
