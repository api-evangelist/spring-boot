---
title: "How to dynamically select a TreeRepository bean at runtime in Spring Boot without a massive switch?"
url: "https://stackoverflow.com/questions/79947131/how-to-dynamically-select-a-treerepository-bean-at-runtime-in-spring-boot-withou"
date: "2026-05-27"
author: "JORGE MARIO CANO COBON"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
I am building a Java Spring Boot application that manages a binary tree structure. Currently, data storage (MongoDB, PostgreSQL, and Memory) and the tree structure (Custom and Collections) are handled differently. For testing, I am changing the strategy by directly editing the pom.xml , but I need a method to handle this dynamically from the UI while the system is running.
