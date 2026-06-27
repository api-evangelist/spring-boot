---
title: "Can't rollback a spring transaction"
url: "https://stackoverflow.com/questions/79965834/cant-rollback-a-spring-transaction"
date: "2026-06-23"
author: "arsrobota"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
In a project I need to import a CSV file into database, and the operation must be rollbacked in the case of any problem. A service calls a helper to read data from file and put them in a List , then it calls a repository extending CrudRepository to persist data with saveAll() . I added @Transactional annotations above the repository's saveAll() and the service's import method.
