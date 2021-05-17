---
title: hugo, github pages를 이용하여 블로그를 만들어 보자
date: 2021-05-17
publishdate: 2021-05-17
draft: true
---

#### 개요
hugo([공식사이트](https://gohugo.io)) SSG(static site generator. [wiki](https://en.wikipedia.org/wiki/Web_template_system#Static_site_generators)) 를 사용 하여 블로그를 만들어 봅시다.
github pages를 이용하여 publish 까지 해봅시다.

#### hugo 설치

hugo를 설치 해야 합니다. [공식사이트](https://gohugo.io/getting-started/installing) 를 참고 하여 설치 합니다. 본인은 macOS 에서 brew를 이용하여 설치 하였습니다.

1. brew 이용하여 설치합니다
```bash
brew install hugo
```

2. 설치가 완료 되었는지 확인 합니다.

```bash
hugo version
> hugo v0.83.1+extended darwin/amd64 BuildDate=unknown
```

3. 블로그 만들기 위한 template 을 생성해줍니다.

```bash
mkdir blog // 디렉토리 생성
cd blog // 생성한 디렉토리로 이동
hugo new site . // 현재 위치에 site template 생성
```
