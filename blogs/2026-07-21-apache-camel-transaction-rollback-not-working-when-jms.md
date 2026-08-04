---
title: "Apache Camel Transaction Rollback Not Working When JMS Reply Queue Fails"
url: "https://stackoverflow.com/questions/79983673/apache-camel-transaction-rollback-not-working-when-jms-reply-queue-fails"
date: "2026-07-21"
author: "MMRahman"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
I'm using Apache Camel with ActiveMQ to process messages in a transactional route. The route receives messages from a queue, performs a database operation, and then sends a response back to a temporary/reply queue. However, when the temporary queue is unavailable or lost during the response phase, the database transaction is already committed , leaving the system in an inconsistent state.
