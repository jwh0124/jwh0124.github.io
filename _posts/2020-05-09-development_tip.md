---
title: Development Tips

categories:
    - DEV
tags:
    - Development

toc: true
toc_sticky: true
toc_label: "페이지 주요 목차"

last_modified_at: 2021-01-07T18:07:00+09:00
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

#### Common Process ####

> 공통 프로세스 리스트 정리, Java 의 경우 AOP로 정의 가능

* 로그인(Session) 관련 처리
* 권한 체크
* XSS (Cross site script) 방어
* Client Program 분기 처리
* Logging
* Transaction
