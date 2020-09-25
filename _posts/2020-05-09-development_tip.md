---
title: Development Tips

categories:
    - DEV
tags:
    - Development

toc: true
toc_sticky: true
toc_label: "페이지 주요 목차"

last_modified_at: 2020-05-09T21:10:00+09:00
---

## Development Tips ##

> 공부하면서 잡다한 팁 정리

### Tips ####

* const : 바뀌지 않는 상수 값 표현, `컴파일 할 때 값이 결정된다.`
* stack : 저장소가 메모리에 할당되는 영역
* heap : 필요에 의해 메모리를 사용하겠다고 요청했을 때 사용할 수 있는 저장소
* 참조 형식 : string, array, class, object
* 값 형식과 참조 형식의 차이점 : 스택에 저장하느냐 힙에 저장하느냐
* 싱글턴 클래스 : 인스턴스가 단 하나만 존재하는 타입
* 정보 은닉(Information Hiding) : 외부에서 멤버 변수를 직접 접근할 수 없게 만드는 것
* as 연산자는 참조형 변수에 대해서만 적용할 수 있다.
* 스레과드는 프로세스 내에서 스택 영역만 따로 할당받고 데이터 영역 힙 영역, 코드 영역은 공유한다.
* var 변수 : 구문상 편의를 위해 사용, 암시적으로 형식화된 지역 변수
* 클래스 스켈레톤 구현 : 리턴 타입을 기본 초기값 위주로 설정 해놓는 것
* 파티셔닝 (partitioning) : 퍼포먼스, 가용성, 정비용이성을 목적으로 당신의 논리적인 데이터 엘리먼트들을 다수의 엔티티로 쪼개는 행위
* 샤딩 (sharding) : 하나로 구성 될 스키마를 다수의 복제본으로 구성
* Thread CPU 점유율 관리 : Thread Sleep 을 통해 낮출 수 있다.

#### Common Process ####

> 공통 프로세스 리스트 정리, Java 의 경우 AOP로 정의 가능

* 로그인(Session) 관련 처리
* 권한 체크
* XSS (Cross site script) 방어
* Client Program 분기 처리
* Logging
* Transaction
