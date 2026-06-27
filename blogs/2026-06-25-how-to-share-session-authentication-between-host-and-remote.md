---
title: "How to share session authentication between host and remote in Module Federation 2.x (Vite) when remoteEntry.js returns 401"
url: "https://stackoverflow.com/questions/79966733/how-to-share-session-authentication-between-host-and-remote-in-module-federation"
date: "2026-06-25"
author: "Lalinda"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
I have a micro-frontend setup using @module-federation/vite (Module Federation 2.x runtime, version 2.5.0): Host app : Pure frontend (React + Vite), no backend Remote app : React + Vite frontend, backed by a Spring Boot backend secured with Spring Security (LDAP-based session auth) Both apps are deployed on the same parent domain (e.g. *.gcrm.example.io ). Problem When the host app loads, it tries to fetch remoteEntry.js from the remote.
