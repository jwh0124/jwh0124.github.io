---
title: Web Server Security

categories:
  - Dev
tags:
  - Web
  - Security
  
toc: true
toc_sticky: true
toc_label: "페이지 주요 목차"

last_modified_at: 2021-06-18T09:34:00+09:00
---

## Web Server Security ##

> Web Server에서 적용 가능한 Security 목록

### Security Terms ###

- 접근 주체 (Principal) : 보호된 리소스에 접근하는 대상
- 인증 (Authentication) : 보호된 리소스에 접근한 대상에 대해 이 유저가 누구인지, 애플리케이션의 작업을 수행해도 되는 주체인지 확인하는 과정
- 인가 (Authorize) : 해당 리소스에 대해 접근 가능한 권한을 가지고 있는 확인하는 과정
- 권한 : 어떠한 리소스에 대한 접근 권한, 모든 리소스는 접근 제어 권한이 걸려있다.

### Security List ###

- csrf (Cross Site Request Forgery) : 사용자가 자신의 의지와는 무관하게 공격자가 의도한 행위를 특정 웹사이트에 요청하게 하는 공격
- HSTS (HTTP Strict Transport Security) : HTTPS Protocol로만 접속하게 하는 기능
- XSS (Cross Site Script) : 관리자가 아닌 권한이 없는 사용자가 웹 사이트에 스크립트를 삽입하는 공격 기법
- HttpFirewall : HttpServlet Request/Response에 방화벽 기능 추가
- SOP (Same Origin Policy) : 다른 출처의 리소스를 사용하는 것에 제한하는 보안 방식
- CORS (Cross-Origin Resource Sharing) : 다른 출처의 자원을 공유
- SQL Injection : 악의적인 SQL 문을 실행되게 함으로써 데이터베이스를 비정상적으로 조작하는 공격 기법
