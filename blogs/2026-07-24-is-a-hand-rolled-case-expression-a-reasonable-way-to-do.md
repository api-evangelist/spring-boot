---
title: "Is a hand-rolled CASE expression a reasonable way to do relevance-ranked search with JPA Criteria API + MySQL, or is there a better approach?"
url: "https://stackoverflow.com/questions/79985518/is-a-hand-rolled-case-expression-a-reasonable-way-to-do-relevance-ranked-search"
date: "2026-07-24"
author: "Dulsara Manakal"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
I'm building a company search endpoint in a Spring Boot app (JPA Criteria API, MySQL) where I want exact matches to appear before prefix matches and before substring matches when a user searches by company name. Right now I'm doing this with a CASE expression built via CriteriaBuilder , used purely for ORDER BY (the actual filtering is a separate LIKE '%keyword%' in the WHERE clause): Expression relevanceRank = cb. selectCase() .when(cb.equal(cb.lower(name), normalizedKeyword), 0) .when(cb.like(cb.lower(name), escapedKeyword + "%", '\\'), 1) .otherwise(2); orders.add(cb.asc(relevanceRank)); Th
