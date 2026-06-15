---
title: "Designing a clean adapter API when an external service supports multiple identifier formats"
url: "https://stackoverflow.com/questions/79954372/designing-a-clean-adapter-api-when-an-external-service-supports-multiple-identif"
date: "2026-06-09"
author: "Dilruk Jayasinghe"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
I have an external service adapter that retrieves a user profile: UserProfileDto getUserProfile(String profileId); The underlying service accepts multiple identifier formats through the same parameter, for example: userId SIN::accountId 94::phoneNumber Because the API accepts a generic String , callers throughout the codebase often build these values manually: getUserProfile("SIN::" + accountId); or getUserProfile(countryCode + "::" + phoneNumber); This has led to identifier formatting logic being scattered across the codebase, and it's not obvious which identifier types are actually supported
