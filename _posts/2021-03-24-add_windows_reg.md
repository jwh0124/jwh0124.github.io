---
title: Add windows registry

categories:
  - Dev
tags:
  - Command
  - windows
  
toc: true
toc_sticky: true
toc_label: "페이지 주요 목차"

last_modified_at: 2021-03-24T19:18:00+09:00
---

## Add windows registry ##

> Windows (OS)에 Registry 추가

### Flow ###

```bash
windows key + R
regedit
move path : HKEY_LOCAL_MACHINE → SOFTWARE → Microsoft → Windows → CurrentVersion → App Paths
add key : execution file (.exe)
example)
  - default value : 'C:\Users\jwh01\Desktop\private\Circle Jung'
  - define path : 'C:\Users\jwh01\Desktop\private'
```
