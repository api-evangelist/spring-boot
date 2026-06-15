---
title: "How to design a maintainable fallback pipeline for classifying bank transactions from different statement formats?"
url: "https://stackoverflow.com/questions/79956785/how-to-design-a-maintainable-fallback-pipeline-for-classifying-bank-transactions"
date: "2026-06-11"
author: "Nikita"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
I am building a Java/Spring application that imports and parses bank statements from different banks. Each bank provides slightly different transaction data. After parsing, I normalize raw bank rows into a common object similar to this: public record ParsedTransaction( LocalDate transactionDate, BigDecimal amount, String merchantName, String description, String bankCategoryName, String mccCode, String transactionTypeCode ) {} The problem is that not all fields are always available: Some banks provide a category, for example Groceries , Transport , Restaurants .
