# Spring Boot

Spring Boot is an open source Java-based framework used to create stand-alone, production-grade Spring-based applications with minimal configuration. It provides auto-configuration, embedded server support, opinionated defaults, and production-ready features including health checks, metrics, and externalized configuration management.

**URL:** https://spring.io/projects/spring-boot

## Tags

Auto Configuration, Embedded Server, Framework, Java, Microservices, REST API, Spring, Web Development

## APIs

### Spring Boot Actuator API

Production-ready management and monitoring endpoints for Spring Boot applications. Provides health checks, metrics, environment info, configuration properties, thread dumps, heap dumps, logger configuration, cache management, and graceful shutdown.

**Human URL:** https://docs.spring.io/spring-boot/docs/current/reference/html/actuator.html
**Base URL:** http://localhost:8080/actuator

**Tags:** Actuator, Health Check, Management, Metrics, Monitoring

**Properties:**
- [Documentation](https://docs.spring.io/spring-boot/docs/current/actuator-api/htmlsingle/)
- [OpenAPI](openapi/spring-boot-actuator-openapi.yml)
- [JSON Schema - Health](json-schema/spring-boot-actuator-health-schema.json)
- [JSON Schema - Metric](json-schema/spring-boot-actuator-metric-schema.json)
- [JSON Structure](json-structure/spring-boot-actuator-structure.json)
- [JSON-LD Context](json-ld/spring-boot-context.jsonld)
- [Spectral Rules](rules/spring-boot-actuator-rules.yml)
- [Naftiko Capability](capabilities/application-monitoring.yaml)

### Spring Boot REST API

RESTful web services built with Spring Boot using Spring MVC or Spring WebFlux. Supports JSON, XML, and hypermedia responses with full content negotiation, validation, error handling, and CORS configuration.

**Human URL:** https://spring.io/guides/gs/rest-service/

**Tags:** HTTP, JSON, REST, Web Services

**Properties:**
- [Documentation](https://docs.spring.io/spring-boot/docs/current/reference/html/web.html)
- [Getting Started Guide](https://spring.io/guides/gs/rest-service/)
- [Tutorial](https://spring.io/guides/tutorials/rest/)

### Spring Data REST API

Exposes Spring Data repositories as hypermedia-driven RESTful resources automatically. Supports HAL, collection+json media types, sorting, pagination, projections, and custom event handlers.

**Human URL:** https://spring.io/projects/spring-data-rest

**Tags:** Database, HATEOAS, Repository, REST

**Properties:**
- [Documentation](https://docs.spring.io/spring-data/rest/docs/current/reference/html/)
- [API Guide](https://docs.spring.io/spring-data/rest/docs/current/api/)
- [Getting Started](https://spring.io/guides/gs/accessing-data-rest/)

### Spring Boot Admin API

Admin UI and monitoring tool for Spring Boot applications providing registration, health monitoring, log level management, JMX bean access, and notification capabilities for multiple application instances.

**Human URL:** https://github.com/codecentric/spring-boot-admin

**Tags:** Administration, Dashboard, Management, Monitoring

**Properties:**
- [Documentation](https://codecentric.github.io/spring-boot-admin/current/)
- [GitHub Repository](https://github.com/codecentric/spring-boot-admin)
- [Getting Started](https://codecentric.github.io/spring-boot-admin/current/#getting-started)

## Artifacts

### OpenAPI Specifications

| Spec | Description |
|------|-------------|
| [spring-boot-actuator-openapi.yml](openapi/spring-boot-actuator-openapi.yml) | Spring Boot Actuator management and monitoring endpoints |

### JSON Schemas

| Schema | Description |
|--------|-------------|
| [spring-boot-actuator-health-schema.json](json-schema/spring-boot-actuator-health-schema.json) | Actuator health response schema |
| [spring-boot-actuator-metric-schema.json](json-schema/spring-boot-actuator-metric-schema.json) | Actuator metric response schema |
| [spring-boot-application-properties.json](json-schema/spring-boot-application-properties.json) | Application configuration properties schema |

### JSON Structures

| Structure | Description |
|-----------|-------------|
| [spring-boot-actuator-structure.json](json-structure/spring-boot-actuator-structure.json) | Actuator API response structure documentation |

### JSON-LD Contexts

| Context | Description |
|---------|-------------|
| [spring-boot-context.jsonld](json-ld/spring-boot-context.jsonld) | Spring Boot linked data context |

### Examples

| Example | Description |
|---------|-------------|
| [spring-boot-actuator-get-health-example.json](examples/spring-boot-actuator-get-health-example.json) | Get application health status |
| [spring-boot-actuator-get-metrics-example.json](examples/spring-boot-actuator-get-metrics-example.json) | Get JVM memory usage metric |
| [spring-boot-actuator-set-logger-example.json](examples/spring-boot-actuator-set-logger-example.json) | Set logger level at runtime |

### Spectral Rules

| Ruleset | Description |
|---------|-------------|
| [spring-boot-actuator-rules.yml](rules/spring-boot-actuator-rules.yml) | API design rules for Spring Boot Actuator conventions |

### Naftiko Capabilities

| Capability | Description |
|------------|-------------|
| [capabilities/application-monitoring.yaml](capabilities/application-monitoring.yaml) | Application monitoring workflow (health, metrics, logs, caches) |
| [capabilities/shared/spring-boot-actuator.yaml](capabilities/shared/spring-boot-actuator.yaml) | Shared Actuator API consumer definition |

### Vocabulary

| Vocabulary | Description |
|------------|-------------|
| [spring-boot-vocabulary.yml](vocabulary/spring-boot-vocabulary.yml) | Spring Boot domain vocabulary and terminology |

## Common Properties

- [Documentation](https://docs.spring.io/spring-boot/)
- [Website](https://spring.io/projects/spring-boot)
- [GitHub](https://github.com/spring-projects/spring-boot)
- [GitHub Organization](https://github.com/spring-projects)
- [Issues](https://github.com/spring-projects/spring-boot/issues)
- [Releases](https://github.com/spring-projects/spring-boot/releases)
- [Stack Overflow](https://stackoverflow.com/questions/tagged/spring-boot)
- [Blog](https://spring.io/blog/category/spring-boot)
- [Guides](https://spring.io/guides)
- [Maven Repository](https://mvnrepository.com/artifact/org.springframework.boot/spring-boot)
- [Spring Initializr](https://start.spring.io/)

## Maintainers

**Name:** VMware Tanzu (Spring Team)  
**Email:** spring-boot@vmware.com  
**URL:** https://spring.io/team
