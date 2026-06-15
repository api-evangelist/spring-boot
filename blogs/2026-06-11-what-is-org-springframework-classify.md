---
title: "What is org.springframework.classify.BinaryExceptionClassifier replacement in spring boot 4/spring 7"
url: "https://stackoverflow.com/questions/79956565/what-is-org-springframework-classify-binaryexceptionclassifier-replacement-in-sp"
date: "2026-06-11"
author: "Dragas"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
Currently I'm upgrading my application to support spring boot 4 (spring 7) and in the migration guide there's a note that spring retry module was replaced by general spring resiliance features, but the migration guide fails to mention what are the actual equivalents and replacements for the said module. For example: https://github.com/spring-projects/spring-boot/wiki/Spring-Boot-4.0-Migration-Guide#spring-kafka-retry-features but it doesn't specify a replacement for org.springframework.classify.BinaryExceptionClassifier which was previously exposed by org.springframework.kafka.listener.Default
