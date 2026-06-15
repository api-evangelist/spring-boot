---
title: "Why does OncePerRequestFilter execute on permitAll() endpoints even when added via addFilterBefore in a SecurityFilterChain?"
url: "https://stackoverflow.com/questions/79958786/why-does-onceperrequestfilter-execute-on-permitall-endpoints-even-when-added-v"
date: "2026-06-14"
author: "Hi Byee"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
I have a Spring Security configuration with a SecurityFilterChain that uses authorizeHttpRequests to permit certain endpoints like /user/register without authentication. However I also have a custom JWT filter added via addFilterBefore(jwtFilter, UsernamePasswordAuthenticationFilter.class) which still executes on those permitAll() endpoints and throws a JWTDecodeException since there is no token present on public endpoints like register and login. I fixed this by adding shouldNotFilter() to my OncePerRequestFilter to explicitly skip those paths, but I don't fully understand why this is necessa
