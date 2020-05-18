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
