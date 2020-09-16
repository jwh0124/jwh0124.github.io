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

#### MVC Pattern ####

### Controller Component ###

- 요청 수락
- 요청에 따른 공통 연산 수행
- 적절한 요청 핸들러 선택
- 핸들러가 관련 비즈니스 로직을 수행할 수 있도록 요청 라우팅
- 오류나 예외 처리를 위한 최상위 핸들러 제공
