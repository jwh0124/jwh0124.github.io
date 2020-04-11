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

### Entity Framework DbContext ###
