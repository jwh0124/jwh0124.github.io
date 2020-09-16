---
title: Design Pattern

categories:
  - Dev
tags:
  - Pattern
  
toc: true
toc_sticky: true
toc_label: "페이지 주요 목차"

last_modified_at: 2020-09-16T13:12:00+09:00
---

## Design Pattern ##

> Design Pattern

### Design Pattern List ###

- MVC Pattern : Model-View-Controller Pattern
- Inversion of Control (IoC) Pattern : 핸들러 객체를 등록해두고, 이벤트 발생 시 특정 메소드 호출
- Strategy Pattern : 알고리즘군을 정의하고 각각을 캡슐화하여 교환해서 사용할 수 있도록 만든다.
- Observer Pattern : 한 객체의 상택다 바뀌면 그 객체에 의존하는 다른 객체들한테 연락이 가고 자동으로 내용이 갱신되는 방식, 일대다 의존성을 정의

#### MVC Pattern ####

### Controller Component ###

- 요청 수락
- 요청에 따른 공통 연산 수행
- 적절한 요청 핸들러 선택
- 핸들러가 관련 비즈니스 로직을 수행할 수 있도록 요청 라우팅
- 오류나 예외 처리를 위한 최상위 핸들러 제공
