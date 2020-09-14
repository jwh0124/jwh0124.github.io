---
title: JUnit Setting

categories:
  - Dev
tags:
  - Java
  - JUnit

toc: true
toc_sticky: true
toc_label: "페이지 주요 목차"

last_modified_at: 2019-12-05T12:43:00+09:00
---

## JUnit ##

### About Junit ###

> 자바 언어를 위한 단위 테스팅 도구

### JUnit - Maven Projects ###

#### pom.xml ####

```bash
<dependency>
    <groupId>junit</groupId>
    <artifactId>junit</artifactId>
    <version>4.12</version>
    <scope>test</scope>
</dependency>
```

### 단위 테스트 프레임워크 규칙 ###

- 단위 테스트는 다른 모든 단위 테스트들과 독립적으로 실행되어야 한다.
- 프레임워크는 테스트 각각의 오류를 식별하고 보고해야 한다.
- 어떤 테스트를 실행할지 선택하기 쉬워야 한다.

### 테스트 클래스가 되는 조건 ###

- public 클래스여야 한다.
- 파라미터를 받지 않는 생성자를 제공해야 한다.
- 반환형은 void 여야 한다.

### Test Definition ###

- Test Class : @Test가 부여된 테스트를 하나 이상 포함한 클래스
- Test Suite : Test들의 집합
- Test Runner : 테스트 스위트 실행 엔진

### 현재 버전 ###

- 4.12

### Reference URL ###

- <https://en.wikipedia.org/wiki/JUnit>

### TODO ###

- JUnit Definition
- Add Example
