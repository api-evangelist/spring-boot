---
title: "Is it possible to get PasswordEncoder bean from UserDetailsService bean?"
url: "https://stackoverflow.com/questions/79954685/is-it-possible-to-get-passwordencoder-bean-from-userdetailsservice-bean"
date: "2026-06-09"
author: "haoz"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
Probably most of the Spring Boot applications developers know it and use it in their WebSecurityConfigurerAdapter extensions: @Override public void configure(AuthenticationManagerBuilder auth) throws Exception { auth.userDetailsService(userDetailsService).passwordEncoder(passwordEncoder()); } but has anyone investigated the possibility of the default passwordEncoder bean extraction from the userDetailsService after set it in this way as above? If the passwordEncoder bean were needed in userDetailService , it would seem unnecessary to inject the bean into userDetailService , which has already b
