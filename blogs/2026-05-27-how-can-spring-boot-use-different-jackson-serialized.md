---
title: "How can Spring Boot use different Jackson serialized ObjectMappers for different controllers?"
url: "https://stackoverflow.com/questions/79947280/how-can-spring-boot-use-different-jackson-serialized-objectmappers-for-different"
date: "2026-05-27"
author: "accbear"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
Background: This is an older Spring Boot 2.4.5 project. A new module related to the intelligent agent API has been added. We want to standardize the JSON format of the API returns for all controllers in the `com.xxx.controller.agent` directory, but without affecting the JSON return values ​​of older controllers.
