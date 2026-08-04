---
title: "Importing proto files from external module for Spring boot gRPC"
url: "https://stackoverflow.com/questions/79980428/importing-proto-files-from-external-module-for-spring-boot-grpc"
date: "2026-07-13"
author: "Oskar"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
Im trying to make project that will share .proto contracts across multiple services. Currently I have made a example contract project: 4.0.0 com.example grpc_contract 1.0-SNAPSHOT 25 25 UTF-8 src/main/proto **/*.proto With one .proto file: src/main/proto/hello.proto . I tried to include this in client project like this: com.example grpc_contract 1.0-SNAPSHOT But during the project installation none sources from .proto files are generated.
