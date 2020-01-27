---

title: App Properties

categories:
    - DEV
tags: 
    - JAVA
    - JPA
    - DB

toc: true
toc_sticky: true
toc_label: "페이지 주요 목차"

last_modified_at: 2020-01-17T18:00:00
---

## Used Application Properties ##

### Classification ###

#### Datasource Attribute ####
- spring.datasource.driverClassName : Database Connection Driver (org.postgresql.Driver)
- spring.datasource.url : Database Connection URL (jdbc:postgresql://localhost:5432/DBName)
- spring.datasource.username : Database Connection User ID (postgres)
- spring.datasource.password : Database Connection Password (password)

#### Hibernate, JPA Attribute ####
- spring.jpa.generate-ddl : 서버 시작 지점에 DDL 문을 생성하여 DB 적용 (true/false)
- spring.jpa.hibernate.ddl-auto : 상세한 데이터베이스 초기화 전략 (none/create-drop/create/update/validate)
- spring.jpa.properties.hibernate.show_sql : Hibernate 가 실행하는 모든 SQL 출력
- spring.jpa.properties.hibernate.format_sql : SQL 문을 보기 좋게 출력 (true/false)