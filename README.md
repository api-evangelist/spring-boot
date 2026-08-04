# Spring Boot (spring-boot)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Spring Boot is an open source Java-based framework used to create stand-alone, production-grade Spring-based applications with minimal configuration. It provides auto-configuration, embedded server support, opinionated defaults, and production-ready features including health checks, metrics, and externalized configuration management.

**APIs.json:** [https://spring.io/projects/spring-boot](https://spring.io/projects/spring-boot)

## Tags

- Auto Configuration
- Embedded Server
- Framework
- Java
- Microservices
- REST API
- Spring
- Web Development

## Timestamps

- **Created:** 2024-01-01
- **Modified:** 2026-05-19

## APIs

### Spring Boot Actuator API

Production-ready management and monitoring endpoints for Spring Boot applications. Provides health checks, metrics, environment info, configuration properties, thread dumps, heap dumps, logger configuration, cache management, and graceful shutdown.

- **Human URL:** [https://docs.spring.io/spring-boot/docs/current/reference/html/actuator.html](https://docs.spring.io/spring-boot/docs/current/reference/html/actuator.html)
- **Base URL:** `http://localhost:8080/actuator`

#### Tags

- Actuator
- Health Check
- Management
- Metrics
- Monitoring

#### Properties

- [Documentation](https://docs.spring.io/spring-boot/docs/current/actuator-api/htmlsingle/)
- [OpenAPI](openapi/spring-boot-actuator-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/spring-boot-actuator.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/spring-boot-actuator.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/spring-boot-actuator-health-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/spring-boot-actuator-metric-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/spring-boot-actuator-structure.json)
- [J S O N L D Context](json-ld/spring-boot-context.jsonld)
- [Spectral Rules](rules/spring-boot-actuator-rules.yml)

### Spring Boot REST API

RESTful web services built with Spring Boot using Spring MVC or Spring WebFlux. Supports JSON, XML, and hypermedia responses with full content negotiation, validation, error handling, and CORS configuration.

- **Human URL:** [https://spring.io/guides/gs/rest-service/](https://spring.io/guides/gs/rest-service/)
- **Base URL:** `http://localhost:8080/api`

#### Tags

- HTTP
- JSON
- REST
- Web Services

#### Properties

- [Documentation](https://docs.spring.io/spring-boot/docs/current/reference/html/web.html)
- [Getting  Started  Guide](https://spring.io/guides/gs/rest-service/)
- [Tutorial](https://spring.io/guides/tutorials/rest/)
- [Postman Collection](collections/spring-boot-actuator.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/spring-boot-actuator.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Spring Data REST API

Exposes Spring Data repositories as hypermedia-driven RESTful resources automatically. Supports HAL, collection+json media types, sorting, pagination, projections, and custom event handlers.

- **Human URL:** [https://spring.io/projects/spring-data-rest](https://spring.io/projects/spring-data-rest)
- **Base URL:** `http://localhost:8080/`

#### Tags

- Database
- HATEOAS
- Repository
- REST

#### Properties

- [Documentation](https://docs.spring.io/spring-data/rest/docs/current/reference/html/)
- [A P I  Guide](https://docs.spring.io/spring-data/rest/docs/current/api/)
- [Getting Started](https://spring.io/guides/gs/accessing-data-rest/)
- [Postman Collection](collections/spring-boot-actuator.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/spring-boot-actuator.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Spring Boot Admin API

Admin UI and monitoring tool for Spring Boot applications providing registration, health monitoring, log level management, JMX bean access, and notification capabilities for multiple application instances.

- **Human URL:** [https://github.com/codecentric/spring-boot-admin](https://github.com/codecentric/spring-boot-admin)
- **Base URL:** `http://localhost:8080/admin`

#### Tags

- Administration
- Dashboard
- Management
- Monitoring

#### Properties

- [Documentation](https://codecentric.github.io/spring-boot-admin/current/)
- [GitHub Repository](https://github.com/codecentric/spring-boot-admin)
- [Getting Started](https://codecentric.github.io/spring-boot-admin/current/#getting-started)
- [Postman Collection](collections/spring-boot-actuator.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/spring-boot-actuator.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Documentation](https://docs.spring.io/spring-boot/)
- [Website](https://spring.io/projects/spring-boot)
- [Git Hub](https://github.com/spring-projects/spring-boot)
- [GitHub Organization](https://github.com/spring-projects)
- [Issues](https://github.com/spring-projects/spring-boot/issues)
- [Releases](https://github.com/spring-projects/spring-boot/releases)
- [Stack Overflow](https://stackoverflow.com/questions/tagged/spring-boot)
- [Blog](https://spring.io/blog/category/spring-boot)
- [Guides](https://spring.io/guides)
- [Maven  Repository](https://mvnrepository.com/artifact/org.springframework.boot/spring-boot)
- [Maven  Central](https://search.maven.org/artifact/org.springframework.boot/spring-boot)
- [Spring  Initializr](https://start.spring.io/)
- [Vocabulary](vocabulary/spring-boot-vocabulary.yml)

## Maintainers

**FN:** VMware Tanzu (Spring Team)
**Email:** spring-boot@vmware.com
**URL:** https://spring.io/team
