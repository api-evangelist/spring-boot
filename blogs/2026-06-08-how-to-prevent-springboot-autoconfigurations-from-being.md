---
title: "How to prevent SpringBoot autoconfigurations from being loaded via component scanning?"
url: "https://stackoverflow.com/questions/79952870/how-to-prevent-springboot-autoconfigurations-from-being-loaded-via-component-sca"
date: "2026-06-08"
author: "fml2"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
This question is a sequel of the SpringBoot issue 50649 (since issues are not a good place to have discussions, I send the question here). The springboot documentation states : Auto-configurations must be loaded only by being named in the imports file. Make sure that they are defined in a specific package space and that they are never the target of component scanning.
