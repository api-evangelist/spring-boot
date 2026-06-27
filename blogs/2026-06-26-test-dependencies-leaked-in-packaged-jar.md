---
title: "Test dependencies leaked in packaged jar"
url: "https://stackoverflow.com/questions/79968354/test-dependencies-leaked-in-packaged-jar"
date: "2026-06-26"
author: "Benoit LEFEVRE -CAMPUS-"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
I recently bootstrapped a small Spring Boot app using IntelliJ's Spring Boot project starter I eventually ended up with the following pom file, after adding two Gatling test dependencies: 4.0.0 org.springframework.boot spring-boot-starter-parent 4.0.6 com.test.dummy test 0.0.1-SNAPSHOT test test 25 3.14.9 org.springframework.boot spring-boot-starter-webmvc-test test org.springframework.boot spring-boot-starter-webmvc io.gatling gatling-app ${gatling.version} test io.gatling.highcharts gatling-charts-highcharts ${gatling.version} test org.springframework.boot spring-boot-maven-plugin What is pu
