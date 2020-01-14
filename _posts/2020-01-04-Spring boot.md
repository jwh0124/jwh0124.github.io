---
title: Spring Boot

categories:
    - Dev
tags:
    - Java
    - Spring
    - Spring Boot

toc: true
toc_sticky: true
toc_label: "페이지 주요 목차"

late_modified_at: 2020-01-04T16:00:00
---

## Spring Boot ##

### Spring Boot 란 ? ###
> 실행만 하면 스프링 기반의 상용화가 가능한 애플리케이션을 쉽게 만들 수 있도록 만든 스프링 프레임워크.


### Spring Boot 특징 ###
- 단독 실행(Stand-alone) 가능
- 내장된 톰캣, 제티 등의 서버를 이용하여 별도의 서버 설치 없이 실행 가능
- 자동화 된 설정 방식 제공

### DI (Dependency Injection) ###
- 프로그래밍에서 구성 요소간에 의존 관계가 소스코드 내부가 아닌 외부의 설정파일 등을 통해 정의되게 하는 패턴
- DI 컨테이너에서 명시적으로 Bean 을 가져오는 방법 : ConfigurableApplicationContext.getBean()

#### DI 적용 유형 ####
- 생성자 주입 : 필요한 의존성을 모두 포함하는 클래스의 생성자를 만들고 그 생성자를 통해 의존성을 주입 
- Setter를 통한 주입 : 의존성을 입력받는 Setter Method를 만들고 이를 통해 의존성을 주입
- Interface를 통한 주입 : 의존성을 주입하는 함수를 포함한 인터페이스를 작성하고 이 인터페이스를 구현하도록 함으로써 실행시에 의존성을 주입

### IOC Container  ###
> IOC (Inversion of Control) 를 구현하는 프레임워크로 객체를 관리하고, 객체의 생성을 책임지고, 의존성을 관리하는 Container

### Component Scan 의 대상이 되는 Annotation ###
> @Component, @Controller, @Service, @Repository, @Configuration

### H2 Database ###
> 자바로 구현한 관계형 데이터베이스 시스템, 내장 DB (설치 작업 없이도 사용 가능)




