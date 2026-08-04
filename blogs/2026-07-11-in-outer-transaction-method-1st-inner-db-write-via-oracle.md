---
title: "In outer transaction method, 1st inner DB write via Oracle SP not rolled back after exception in 2nd inner one"
url: "https://stackoverflow.com/questions/79979923/in-outer-transaction-method-1st-inner-db-write-via-oracle-sp-not-rolled-back-af"
date: "2026-07-11"
author: "gene b."
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
I can't figure out what I'm missing and Google AI also hasn't helped (I pass both of the requirements of [1] No self-invocation and [2] No swallowing of exceptions in the outer transaction method). I have an outer transaction method, performDBWrites() , which calls 2 inner transaction methods that call Oracle stored procedures, responseService.createResponse(..) and responseService.updateResponse(..) . The 2 inner transaction methods are propagation=Propagation.REQUIRED, readOnly=false, rollbackFor=Exception.class .
