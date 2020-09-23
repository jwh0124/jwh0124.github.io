---
title: Dotnet Annotation

categories:
    - Dev
tags:
    - Dotnet
    - Entity Framework Core

toc: true
toc_sticky: true
toc_label: "페이지 주요 목차"

late_modified_at: 2020-06-02T23:00:00+0900
---

## Used Dotnet Annotation ##

### EntityFramework Core ###

> EntityFramework Core 개발 시 사용한 Annotation

| Annotation | Description |
| :--- | :--------------------------------------------------------- |
| `[DatabaseGenerated]` | 데이터베이스에서 속성 값을 생성하는 방법을 지정합니다. (None, Identity, Computed) |
| `[Table]` | 테이블 선언 Annotation |
| `[ProducesResponseType]` | 응답, 스키마 및 매개 변수 메타데이터를 사용하도록 지원하고 보강하는 확장을 제공 |
| `[Key]` | 엔터티의 기본 키 |
| `[MaxLength]` | 엔터티의 MaxLength Validation |
| `[MinLength]` | 엔터티의 MinLength Validation |
| `[Column]` | 엔터티의 Attribute, Column Name 및 Type 정의 가능 |
| `[NotMapped]` | 모델에 형식을 포함하지 않을 경우 사용, Not Table Mapping |
| `[ForeignKey]` | 외래키 Mapping |
| `[Fact]` | xunit Test Case |
| `[Trait]` | xunit Test Description |
