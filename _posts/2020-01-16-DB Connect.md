---

title : DB Connect

categories:
    - DEV
tags:
    - JAVA
    - DataBase

toc: true
toc_sticky: true
toc_label: "페이지 주요 목차"

last_modified_at: 2020-01-16T22:30:00
---

## DB Connect ##

> Java Database Connect

### PostgreSQL DB Connection ###

#### 의존성 추가 ####

```
<dependency>
    <groupId>org.postgresql</groupId>
    <artifactId>postgresql</artifactId>
</dependency>
```

#### Spring Boot Application Properties config ####

```
spring.datasource.hikari.maximum-pool-size=4

spring.datasource.url=jdbc:postgresql://localhost:5432/springboot
spring.datasource.username=add
spring.datasource.password=pass
```

