---
title: "Duplicate default methods inherited from two generated OpenAPI interfaces in Spring Boot [duplicate]"
url: "https://stackoverflow.com/questions/79946622/duplicate-default-methods-inherited-from-two-generated-openapi-interfaces-in-spr"
date: "2026-05-26"
author: "JEINER ANDY JOSUE PINEDA CORLE"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
I am working with OpenAPI-generated interfaces in Spring Boot. My controller implements two generated interfaces: public class TreeController implements NodesApi, TreeApi { However, I get this compilation error: Duplicate default methods named getRequest with the parameters () and () are inherited from the types TreeApi and NodesApi Both interfaces were generated automatically from my OpenAPI specification. What I already tried: I checked both interfaces and they contain similar default methods.
