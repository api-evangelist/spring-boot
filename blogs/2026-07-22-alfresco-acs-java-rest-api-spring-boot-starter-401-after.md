---
title: "Alfresco ACS Java REST API Spring Boot Starter: 401 after OAuth2 token expiration during long running jobs"
url: "https://stackoverflow.com/questions/79983771/alfresco-acs-java-rest-api-spring-boot-starter-401-after-oauth2-token-expiratio"
date: "2026-07-22"
author: "Giovanni Leonardo Casagrande"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
I am using Alfresco ACS Java REST API Spring Boot Starter (version 7.1.0) with Keycloak as OAuth2 Identity Provider. The authentication is configured using client_credentials : spring.security.oauth2.client.registration.alfresco-rest-api.authorization-grant-type=client_credentials The Alfresco APIs are injected with @Autowired (i.e. private NodesApi nodesApi ); Short calls work correctly.
