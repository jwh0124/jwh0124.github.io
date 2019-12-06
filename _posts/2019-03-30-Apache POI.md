---
title: Apache POI

categories:
  - Dev
tags:
  - Java
  - Maven
last_modified_at: 2019-12-05T12:43:00+09:00
---



## Apache POI 란? ##

> 아파치 POI (Apache POI) 는 아파치 소프트웨어 재단에서 만든 라이브러리로서 마이크로소프트 오피스 파일 포맷을 순수 자바 언어로서 읽고 쓰는 기능을 제공 POI ( Poor Obfuscation mplementation )

 

## Apache POI 아키텍처 ##
- POIFS(Poor Obfuscation Implementation File System) : 마이크로소프트 오피스의 OLE 2 Compound document 파일 포맷을 읽고 쓰는 컴포넌트. 모든 오피스 파일 포맷은 OLE2 방식이므로 하위 모든 컴포넌트의 기반이 된다.
- HSSF(Horrible SpreadSheet Format) : 마이크로소프트 엑셀 파일포맷을 읽고 쓰는 컴포넌트로서 엑셀 97버전부터 현재까지 지원한다.
- XSSF(XML SpreadSheet Format) : 마이크로소프트 엑셀 2007부터 지원하는 오피스 오픈 XML 파일 포맷인 *.xlsx 파일을 읽고 쓰는 컴포넌트이다.
- HPSF(Horrible Property Set Format) : 오피스 파일의 문서요약 정보를 읽는데 사용되는 컴포넌트이다.
- HSLF(Horrible Slid Layout Format) : 마이크로소프트 파워포인트 파일을 읽고 쓰는데 사용되는 컴포넌트이다.
- HDGF(Horrible DiaGram Format) : 마이크로소프트 비지오 파일을 읽는데 사용하는 컴포넌트이다.
- HPBF(Horrible PuBlisher Format) : 마이크로소프트 퍼블리셔 파일을 다루는데 사용되는 컴포넌트이다.
- HSMF(Horrible PuBlisher Format) : 마이크로소프트 아웃룩에서 사용되는 *.msg 파일을 다루는데 사용되는 컴포넌트이다.
- DDF(Dreadful Drawing Format) : 마이크로소프트 오피스에서 사용되는 이미지 파일을 읽어오는데 사용하는 컴포넌트이다.



## Apache POI - Maven Projects ##

### pom.xml ###
```
<dependency>
  <groupId>org.apache.poi</groupId>
  <artifactId>poi-ooxml</artifactId>
  <version>3.15</version>
</dependency>
```

 

## 현재 버전 ##

- 3.15 

 

## 참고 URL ##

- <https://poi.apache.org/overview.html/>
- 예제 샘플 : <https://gist.github.com/madan712/3912272/>
