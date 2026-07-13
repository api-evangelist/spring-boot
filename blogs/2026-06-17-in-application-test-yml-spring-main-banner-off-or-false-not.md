---
title: "In application-test.yml, spring > main > banner: \"off\" (or false) not turning off Spring Banner in mvn clean install on jUnit execution"
url: "https://stackoverflow.com/questions/79962367/in-application-test-yml-spring-main-banner-off-or-false-not-turning-of"
date: "2026-06-17"
author: "gene b."
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
We are using Spring 3.5.14 and have the 2 standard Spring files main/resources/application.yml test/resources/application-test.yml The goal is to prevent the output of the Spring Banner, but only during the jUnit execution in mvn clean install . If we add the following to the main application.yml , it works, but the banner is also hidden during the application run, which is not what we want. We only want the jUnit suppression of the banner.
