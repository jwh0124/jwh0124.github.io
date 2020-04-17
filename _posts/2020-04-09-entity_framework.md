---
title: Entity Framework

categories: DEV
tags:
    - C Sharp
    - ORM
    - Framework

toc: true
toc_sticky: true
toc_lable: "페이지 주요 목차"

last_modified_at: 2020-04-09T21:49:00
---

## Entity Framework ##

> 개체 관계형 매퍼(O/RM)로, .Net 개발자들이 .Net 개체를 사용하여 DB 작업을 수행할 수 있습니다.

### Entity Framework Model ###

1. Code First : Domain Object 를 먼저 정의하고 프로그램 실행 시 DB가 없으면 자동으로 DB 생성
2. Model First : Entity Framework Designer를 사용하여 모델 추가하여 생성
3. DB First : 기존 데이터 베이스 모델을 리버스 엔지니어링하여 생성

### Entity Framework Core ###

> EF Core는 널리 사용되는 Entity Framework 데이터 액세스 기술의 가볍고 확장 가능한 오픈 소스 플랫폼 교차 버전

#### Entity Framework Core Database Control ####

##### Database CRUD #####

- Migration을 사용하여 데이터베이스 만들기

```bash
Install-Package Microsoft.EntityFrameworkCore.Tools
Add-Migration InitialCreate
Update-Database
```

- Database Update

```bash
Update-Database
```

- Migration Code 지정 : 데이터베이스 스키마가 동기화되지 않을 경우 다른 마이그레이션 코드를 추가하여 Update 필요

```bash
Add-Migration MigrationCode
```

- Migration Delete

```bash
Remove-Migration
```

- Migration Rollback

```bash
Update-Database MigrationCode
```

##### Create SQL Script #####

- Debugging & Deploy 시 생성, Migration Code 별 From, to 사용으로 추가, 롤백 스크립트도 생성 가능

```bash
Script-Migration
```
