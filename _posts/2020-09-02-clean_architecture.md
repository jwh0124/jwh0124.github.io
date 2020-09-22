---
title: Clean Architecture

categories:
  - Dev
tags:
  - Architecture
  
toc: true
toc_sticky: true
toc_label: "페이지 주요 목차"

last_modified_at: 2020-09-02T10:00:00+09:00
---

## Clean Architecture ##

> Clean Architecture Review

### Clean Architecture Definition ###

- 모든 소프트웨어 시스템은 행위와 구조 두 가지 가치를 제공한다.

### Paradigm List ###

- 구조적 프로그래밍 : 제어흐름의 직접적인 전환에 대해 규칙을 부과한다.
- 객체 지향 프로그래밍 : 제어 프름의 간접적인 전환에 대해 규칙을 부과한다.
- 함수형 프로그래밍 : 할당문에 대해 규칙을 부과한다.

### OO (Object-Oriented) ###

> OO 란 : 다형성을 이용하여 전체 시스템의 모든 소스 코드 의존성에 대한 절대적인 제어 권한을 획득 할 수 있는 능력

- 캡슐화 (encapsulation)
- 상속 (inheritance)
- 다형성 (polymorphism)
- OO 지향 (아키텍트 관점) : 의존성을 원하는 방향으로 설정 할 수 있다.

### SOLID 원칙 ###

> 목적 : 변경에 유연하다, 이해하기 쉽다, 시스템에 사용될 수 있는 컴포넌트의 기반이 된다.

- SRP (Single Responsibility Principle) : 단일 책임 원칙, 하나의 모듈은 하나의, 오직 하나의 액터에 대해서만 책임져야 한다.
- OCP (Open-Closed Principle) : 개방-폐쇄 원칙, 소프트웨어 개체는 확장에는 열려 있어야 하고, 변경에는 닫혀 있어야 한다.
- LSP (Liskov Substitution Principle) :  리스코프 치환 원칙
- ISP (Interface Segregation Principle) : 인터페이스 분리 원칙
- DIP (Dependency Inversion Principle) : 의존성 역전 원칙

### 컴포넌트 (Component) ###

> 배포 단위, 시스템의 구성 요소로 배포할 수 있는 가장 작은 단위

- Java : jar
- Ruby : gem
- .Net : dll

### Reference Blog ###

- [Wiki](https://ko.wikipedia.org/wiki/SOLID_(%EA%B0%9D%EC%B2%B4_%EC%A7%80%ED%96%A5_%EC%84%A4%EA%B3%84))
- [SOLID 원칙](https://victorydntmd.tistory.com/291)
