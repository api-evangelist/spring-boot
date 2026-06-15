---
title: "Custom Password validator shows errors randomly in template [closed]"
url: "https://stackoverflow.com/questions/79958481/custom-password-validator-shows-errors-randomly-in-template"
date: "2026-06-13"
author: "IgorArnaut"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
com/example/realestate/dtos/auth/RegisterDTO.java has @Password annotation: @Data @ConfirmPassword public class RegisterDTO { @NotBlank(message = "{email.NotBlank}") @Email(message = "{email.Email}") private String email; @NotBlank(message = "{password.NotBlank}") @Password private String password; private String password2; @NotBlank(message = "{phone.NotBlank}") @Pattern(regexp = "^\\+381 \\d{2} \\d{6,7}$", message = "{phone.Pattern}", groups = AdvancedValidation.class) // ... } com/example/realestate/validators/Password.java : @Documented @Constraint(validatedBy = PasswordConstraint.class) @
