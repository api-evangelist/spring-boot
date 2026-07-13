---
title: "Why does my application return different data than a direct SQL query?"
url: "https://stackoverflow.com/questions/79977784/why-does-my-application-return-different-data-than-a-direct-sql-query"
date: "2026-07-08"
author: "Dharmendra Prajapati"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
I'm facing a strange issue, where the same PostgreSQL function returns different results, when executed from my Java application versus pgAdmin. Environment Spring Boot 3.0.6 PostgreSQL 15.3 JPA EntityManager#createNativeQuery() Same PostgreSQL server, database, schema, and user PostgreSQL Function Call SELECT wisun_get_presence_details_json( '8C73DAFFFE1693AE', 1780857000000, 1783484219909 ); Result from pgAdmin [ {"status":"DISCONNECTED","createdAt":1780857000000}, {"status":"CONNECTED","createdAt":1781670691000}, {"status":"DISCONNECTED","createdAt":1781677649000}, {"status":"CONNECTED","cr
