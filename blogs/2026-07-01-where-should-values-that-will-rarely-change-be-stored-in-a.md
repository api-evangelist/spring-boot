---
title: "Where should values that will rarely change be stored in a full stack application"
url: "https://stackoverflow.com/questions/79972390/where-should-values-that-will-rarely-change-be-stored-in-a-full-stack-applicatio"
date: "2026-07-01"
author: "Tapialj"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
A simple example would be something like Entertainment Software Rating Board (ESRB) ratings, they change on occasion but not often. If I wanted to keep a list of these ratings for a full stack app, where best to store them? I've usually just created a table in my db and pull them through into spring, where needed, and into the front end as needed.
