---
title: "Use custom validators in correct order"
url: "https://stackoverflow.com/questions/79969050/use-custom-validators-in-correct-order"
date: "2026-06-28"
author: "IgorArnaut"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
I have this DTO class that has class-level custom validators, Password and ConfirmPassword , depend on other fields, and I intend to use them on another DTO object. @Data @Builder(toBuilder = true) @Password @ConfirmPassword public class RegisterDTO { @NotBlank(message = "{email.NotBlank}") @Email(message = "{email.Email}") private String email; @NotBlank(message = "{password.NotBlank}") private String password; private String password2; @NotBlank(message = "{phone.NotBlank}") @Pattern(regexp = "^\\+381 \\d{2} \\d{6,7}$", message = "{phone.Pattern}") private String phone; @NotBlank(message = "
