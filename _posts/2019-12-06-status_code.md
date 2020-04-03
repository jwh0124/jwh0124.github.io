---
title: HTTP Status Code

categories:
    - Dev
tags:
    - HTTP

toc: true
toc_sticky: true
toc_label: "페이지 주요 목차"

late_modified_at: 2019-12-06T18:00:00
---

## Used HTTP Status Code ##

### 2xx (Success) ###

| Code | Code Message |
| :--- | :--------------------------------------------------------- |
| `200` | OK, 성공 |
| `201` | Created, 새 리소스 생성 |
| `202` | Accepted, 요청을 접수 했지만 아직 처리되지 않음 |
| `204` | No Content, 요청을 처리했지만 Response Content X |

### 4xx (Request Error) ###

| Code | Code Message |
| :--- | :--------------------------------------------------------- |
| `400` | Bad Request, 잘못된 요청 |
| `401` | Unauthorized, 권한 없음 |
| `402` | Payment Required, 결제 필요 |
| `403` | Forbidden, 서버가 요청 거부(리소스 권한 X) |
| `404` | Not Found, 요청한 페이지를 찾을 수 없다 |

### 5xx (Server Error) ###

| Code | Code Message |
| :--- | :--------------------------------------------------------- |
| `500` | Interal Server Error, 내부 서버 오류 |
| `501` | Not Implemented, 구현되지 않음 |
