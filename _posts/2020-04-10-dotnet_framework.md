---
title: .Net Framework & .Net COre

categories:
    - Dev
tags:
    - C Sharp
    - Framework
    - Dot net
    - Dot net core

toc: true
toc_sticky: true
toc_label: "페이지 주요 목차"

last_modified_at: 2020-04-10T09:33:00
---

## About Framework ##

> 특정 운영체제 기반에서 동작하는 응용 소프트웨어를 쉽게 빠르게 구현하게 하기 위한 클래스와 라이브러리들의 구조적인 모임

### .NET Framework 구조 ###

* 공통 언어 런타임(CLR)  
닷넷 프레임워크의 가장 핵심 기능으로 자바에서의 가상 머신 역할을 한다. GC(Garbage Collector)를 호출하여 동적 할당이 된 메모리를 제거하는 역할도 한다.

* JIT 컴파일러  
C# 코드를 빌드하면 MSIL이라는 중간 코드를 만들어낸다. 이 중간 코드로는 컴퓨터가 읽을 수 없으므로, 프로그램 실행 시 중간 코드는 JIT 컴파일러에 의해 Native 코드로 변경 된다.

### Command 명령어 종류 ###

| 명령어 | 기능 |
| :--------- | :--------- |
| dotnet new | 새로운 프로젝트를 생성한다. |
| dotnet build | 프로젝트를 빌드한다. |
| dotnet run | 프로그램을 실행한다. |
| dotnet publish -r (OS Version) | OS 버전에 따라 컴파일한다. |

### 자료형의 종류 ###

| 자료형 | 내용 |
| :---- | :--- |
| bool | 참인 경우는 true, 거짓인 경우는 false로 표시한다. |
| byte | 1byte의 메모리를 차지하고, 양수만 표현한다. 범위는 0~255이다. |
| sbyte | 1byte의 메모리를 차지하고, 양수와 음수 표현이 모두 가능하다. 범위는 -127~128이다. |
| int | 0을 포함한 양수와 음수의 정수를 표현한다. |
| float | 소수점 7자리까지의 실수를 표현한다. |
| double | 소수점 16자리까지의 실수를 표현한다. |
| char | 문자 1개를 표현한다. |
| string | 여러 개의 문자들로 이루어진 문자열을 표현한다. |
| object | 어떠한 자료형도 표현할 수 있다. |

### 연산자들의 종류 ###

| 기능별 분류 | 연산자 종류 |
| :--------- | :--------- |
| 산술 연산자 | + - * / % |
| 대입 연산자 | = += -= *= /= %= |
| 부호 연산자 | + - |
| 증감 연산자 | ++ -- |
| 관계 연산자 | == != <> <= >= |
| 논리 연산자 | &#124;&#124; && ! |
| 비트 연산자 | ! & >> << ~ |

#### .Net 용어 ####

| 용어 | 내용 |
| :--- | :--- |
| BCL (Base Class Library) | MS에서 미리 만들어 놓은 특정 기능을 수행하는 타입 Library |
| .Net Standard Library | .Net과 .Net Core 사이에 라이브러리의 불일치를 해결하기 위해 만든 Standard Library |
| 직렬화(Serialization) | 객체를 저장하거나 메모리, DB 또는 파일로 전송하기 위해 객체를 byte 스트림으로 변환하는 프로세스 |
| 델리게이트(Delegate) | 특성 메소드의 기능을 대신 위임받아서 처리하는 기능 |

#### C# 식별자 명명 규칙 ####

* 식별자의 시작 문자는 숫자로 시작할 수 없고, 반드시 문자여야 한다.
* 특수 문자 중에서 유일하게 _ 문자을 시작 문자로 사용할 수 있다.
* 유니코드 범위의 문자가 허용되기 떄문에 `한글` 식별자도 가능하다.
* 예약어를 식별자로 사용할 수 없다. 사용해야 한다면 `@` 문자를 접두사로 사용하여 C# 컴파일러가 예약어가 아닌 식별자로 인식하게 할 수 있다.
* 흔한 경우는 아니지만 이스케이프 시퀀스로도 식별자를 사용할 수 있다.

#### 스레드의 4가지 상태 ####

* 생성 직후 (Unstarted) 상태
* 실행 가능 (Runnable) 상태
* 대기 (Suspended) 상태
* 종료 (Stopped) 상태

#### Project Build ####

* dotnet publish -r <빌드할 환경> : dotnet publish -r ubuntu.16.04-arm

#### 환경변수 추가 (Linux 환경) ####

```bash
mkdir -p $HOME/dotnet && tar zxf aspnetcore-runtime-3.1.0-linux-x64.tar.gz -C $HOME/dotnet
export DOTNET_ROOT=$HOME/dotnet
export PATH=$PATH:$HOME/dotnet
```
