---
title: "How do I wait my program thread for something to happen in Spring Boot and then wake it up?"
url: "https://stackoverflow.com/questions/79965097/how-do-i-wait-my-program-thread-for-something-to-happen-in-spring-boot-and-then"
date: "2026-06-22"
author: "malaachi"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
I am writing this backend software where I need to send Firebase notifications to the client (a tablet), and when I send the notification itself (wrapped in a method) I want my thread to wait 10 seconds for the tablet to reply then, if the time has passed without getting a response, he should normally resume its execution but, if tablet reply falls within 10 seconds, I want my thread to wake up. How do I implement this thing? In the project our team is developing, we're using an approach with ThreadPoolTaskExecutor .
