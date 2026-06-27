---
title: "HTTP/2 requests to Spring Boot on ECS behind AWS NLB fail with PROTOCOL_ERROR (HTTP/1.1 works fine)"
url: "https://stackoverflow.com/questions/79966902/http-2-requests-to-spring-boot-on-ecs-behind-aws-nlb-fail-with-protocol-error-h"
date: "2026-06-25"
author: "Auke"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
After upgrading our application to Spring Boot 4.1.0, requests started failing once the service was running behind an AWS Network Load Balancer (NLB) configured with a TLS listener. The same build worked before the upgrade. Our setup terminates (offloads) TLS at the NLB via a TLS listener, and the connection from the NLB to the target group is plain, non-TLS.
