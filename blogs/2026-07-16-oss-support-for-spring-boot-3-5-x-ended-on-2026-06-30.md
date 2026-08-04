---
title: "\"OSS support for Spring Boot 3.5.x ended on 2026-06-30\" message doesn't go away after upgrading to 4.1.0"
url: "https://stackoverflow.com/questions/79981421/oss-support-for-spring-boot-3-5-x-ended-on-2026-06-30-message-doesnt-go-away"
date: "2026-07-16"
author: "g marinedev"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
I migrated from Spring Boot 3.5.x to 4.1.0 with Java 21 and Gradle 9.3.1 in VS Code. Everything seems to work fine, but VS Code still gives me the annoying message: OSS support for Spring Boot 3.5.x ended on 2026-06-30, get commercial support until 2032-06-30 via Tanzu Spring Runtime at https://spring.io/support(BOOT_VERSION_VALIDATION_CODE) I specified Gradle 9.3.1 in the gradle.properties . I the build.gradle file, the first character in plugins has the squiggly underline indicating a problem.
