---
title: 'springboot'
layout: post
tags:
  - development
category: development
---

1) 재기동 없이 class 수정사항 자동 반영하기
pom.xml에서  '<dependency'> 밑에서 ctrl+space를 누른후 [edit starters..]를 더블 클릭 하여 Spring DevTools 체크 하면 아래 의존관계 추가 됨.

``
<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-devtools</artifactId>
			<scope>runtime</scope>
</dependency>
``


2) VO 객체 getter/setter 자동 생성
VO 객체 생성 후 private int seq; 정의 후,
이클립스 alt+shift+S를 이용하여 generate