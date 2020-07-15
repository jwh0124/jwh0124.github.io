---
title: Linux Command

categories:
  - Dev
tags:
  - Linux
  
toc: true
toc_sticky: true
toc_label: "페이지 주요 목차"

last_modified_at: 2020-04-22T10:15:00+09:00
---

## Used Linux Command ##

> Linux Terminal Command List

### Used Linux Command List ###

| Command | Command Description | Option | Option Description |
| :------ | :------------------ | :----- | :----------------- |
| ps | 프로세스 확인(Process Status) | -e | 모든 프로세스 |
| | | -f | Full Format |
| | | -l | Long Format |
| | | p, -p | 특정 PID의 프로세스 |
| | | -u | 특정 사용자의 프로세스 |
| ll | 디렉토리 내용 길게 보기 (ls -l의 별칭) | -a | 숨김 파일까지 조회 |
| chmod | 파일 권한 부여 | | |
| chown | 파일 소유권 변경 | | |
| df | 파일 용량 확인 | | |
| mv | 파일 이동 및 이름 변경 | | |
| cp | 파일 복사 | | |
| systemctl | Service 관리 | start | 서비스 시작
| | | stop | 서비스 종료 |
| | | status | 서비스 상태 조회 |
| ldconfig | ld library reload | | |
| | | -v | 연결 된 ld library 조회 |

### Service Config for linux ###

```bash
[Unit]
Description=Service Description

[Service]
WorkingDirectory=Target service path
ExecStart=Start exec script
SyslogIdentifier=system log identifier

[Install]
WantedBy=multi-user.target
```

### System Loading Script Config ###

> vi ~./bashrc : 환경 변수 및 파일 등 bash가 수행될 때 실행되는 함수를 제어하는 지역적인 시스템 설정과 관련된 파일

### LD_LIBRARY_PATH Config ###

> /etc/ld.so.conf 편집, export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/cubox/Model:/cubox/cubox_api/lib

### Debian Network Setting ###

```bash
vi /etc/network/interfaces

auto eth0
iface eth0 inet static
address 192.168.0.1
netmask 255.255.0.0
gateway 192.168.0.1
dns-nameservers 8.8.8.8
```

#### 설정 파일 적용 ####

```bash
/etc/init.d/networking stop
/etc/init.d/networking start
/etc/init.d/networking restart
```
