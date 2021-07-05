---
title: Development Tips

categories:
    - DEV
tags:
    - Development

toc: true
toc_sticky: true
toc_label: "페이지 주요 목차"

last_modified_at: 2021-02-19T15:07:00+09:00
---

## Development Tips ##

> 공부하면서 잡다한 팁 정리

### Tips ####

* const : 바뀌지 않는 상수 값 표현, `컴파일 할 때 값이 결정된다.`
* stack : 저장소가 메모리에 할당되는 영역, 기능에 의해 생성 된 임시 변수를 저장하는 컴퓨터 메모리 영역, LIFO 자료구조, 개별적인 메모리, 각 함수의 지역변수가 저장되는 공간
* heap : 필요에 의해 메모리를 사용하겠다고 요청했을 때 사용할 수 있는 저장소, 객체를 저장하기 위해 사용, 모든 스레드가 공유하는 메모리
* 참조 형식 : string, array, class, object
* 값 형식과 참조 형식의 차이점 : 스택에 저장하느냐 힙에 저장하느냐
* 싱글턴 클래스 : 인스턴스가 단 하나만 존재하는 타입
* as 연산자는 참조형 변수에 대해서만 적용할 수 있다.
* 스레과드는 프로세스 내에서 스택 영역만 따로 할당받고 데이터 영역 힙 영역, 코드 영역은 공유한다.
* var 변수 : 구문상 편의를 위해 사용, 암시적으로 형식화된 지역 변수
* Thread CPU 점유율 관리 : Thread Sleep 을 통해 낮출 수 있다.
* Maven Scope : Compile (Default)
* Pointer : & (Point), * (Read, Set)
* Function : 독립적으로 존재하며, 로직 처리 이 후 사용자가 원하는 결과를 반환
* Method : 클래스에 종속되어 존재, 해당 클래스에 대한 객체가 생성되어야 사용할 수 있다.
* 설정자 메서드(setter method ) -> Pointer receiver 사용
* nohub : 프로그램과 프로세스가 백그라운드에서 동작하도록 한다.
* new 연산자는 heap 영역에 충분한 공간이 있는지 확인한 후 메모리를 확보하는 역할을 한다.
* NoSQL(Not Only SQL) : 다양한 비정형 데이터 저장, 키-밸류나 문서, 테이블 데이터 간 연결을 고려하는 그래프, 분산형 데이터, `샤드`라는 단위로 분산
* datetime, timestamp : datetime은 timezone을 지원하지 X, 검색 시에도 timestamp가 더 빠름.
* bigint, int : bigint는 8바이트, int는 4바이트 정수값으로 mysql에서 사용하는 메모리 용량이 적어진다.
* equals, == 차이점 : equals는 값을 비교, ==는 객체의 주소값을 비교.
* 기본형 (Primitive type)은  Stack 에 저장, 참조형 (Reference type)은 heap에 저장
* Unix Timestamp 지양 이유 : 2038 Problem을 가지고 있기 때문 -> [비교글](https://velog.io/@lsb156/Instant-vs-LocalDateTime)
* RestAPI 만드는 이유 : Client Side를 정형화된 플랫폼이 아닌 모바일, PC, 어플리케이션 등 플랫폼에 제약을 두지 않기 위해
* 트랜스파일(transpile) : 어떤 프로그래밍 언어로 작성된 코드를 다른 프로그래밍 언어로 된 코드로 변환하는 것
* 스캐폴딩 : 개발을 쉽게 할 수 있도록 도와주는 일련의 자동화 과정
* Spring MVC Controller와 Restful Web Service Controller의 차이점 : HTTP Response Body가 생성되는 방식
* GC 란(Garbage Collector) : 메모리 관리 기법 중에 하나로, 프로그램이 동적으로 할당했던 메모리 영역 중에서 필요없게 된 영역을 해제하는 기능
* CoC (설정보다 관례) : 개발자들에게 결정할 개수를 줄여서 개발을 용이하고 단순하게 하지만 그렇다고 해서 유연성을 잃지 않게 하도록 하는 소프트웨어 디자인 패러다임
* 식별관계 : 부모 테이블의 기본 키를 내려받아서 자식 테이블의 기본 키 + 외래키로 사용하는 관계
* 비식별 관계 : 부모 테이블의 기본 키를 받아서 자식 테이블의 외래 키로만 사용하는 관계
* 자바는 객체에 값을 대입하면 항상 참조값을 전달한다.

#### Common Process ####

> 공통 프로세스 리스트 정리, Java 의 경우 AOP로 정의 가능

* 로그인(Session) 관련 처리
* 권한 체크
* XSS (Cross site script) 방어
* Client Program 분기 처리
* Logging
* Transaction
* Exception Process (AOP, @ControllerAdvice, @ExceptionHandler)

#### Subquery ####

* 스칼라 서브쿼리 : SELETE문에 있는 서브쿼리
* 인라인 뷰 : FROM 절에 있는 서브쿼리
* 서브쿼리 : WHERE 절에 있는 서브쿼리

##### MariaDB Query ANALYZE ####

* ANALYZE FORMAT=JSON "Query"

#### Java Version ####

* Java 10
  * var keywords
  * JVM 힙 영역을 시스템 메모리가 아닌 다른 종류의 메모리에도 할당 가능
  * 병럴 처리 가비지 컬렉션 도입으로 인한 성능 향상
* Java 11
  * The Z Garbage Collector(ZGC) : 대기 시간이 낮은 확장 가능한 GC
  * 람다 파라미터에 대한 지역변수 문법
