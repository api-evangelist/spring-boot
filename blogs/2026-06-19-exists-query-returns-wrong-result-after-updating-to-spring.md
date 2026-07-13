---
title: "Exists query returns wrong result after updating to Spring Boot 4.1"
url: "https://stackoverflow.com/questions/79963016/exists-query-returns-wrong-result-after-updating-to-spring-boot-4-1"
date: "2026-06-19"
author: "Tim Niederhäuser"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
After updating to Spring Boot 4.1 some of our tests fail. The test: @SpringBootTest @Transactional class SpringTestApplicationTests { @Autowired RoleRepository roleRepository; @Autowired UserRepository userRepository; Role role; @BeforeEach public void setUp() { role = new Role(); role.name = "Admin"; role = roleRepository.saveAndFlush(role); } // fails during second assert @Test void test_exists() { assertThat(roleRepository.isRoleReferencedByAnyUser(role.id)).isEqualTo(false); var user = new User(); user.name = "admin"; user.role = role; userRepository.saveAndFlush(user); assertThat(roleRepo
