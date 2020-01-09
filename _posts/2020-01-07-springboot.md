---
title: 'springboot'
layout: post
tags:
  - development
category: development
---

> 재기동 없이 class 수정사항 자동 반영하기
pom.xml에서  `<dependency>` 밑에서 ctrl+space를 누른후 [edit starters..]를 더블 클릭 하여 Spring DevTools 체크 하면 아래 의존관계 추가 됨.

 ```java
<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-devtools</artifactId>
			<scope>runtime</scope>
</dependency>
 ```


> VO 객체 getter/setter 자동 생성
VO 객체 생성 후 private int seq; 정의 후,
이클립스 alt+shift+S를 이용하여 generate

>롬복라이브러리 이용
위의 방법이 소스가 지저분해지고 모든 VO클래스와 JPA사용 도메인 클래스에 메소드 반복작성을 피하기 위해 자바 컴파일 시에 자동으로 생성자 Getter, Setter, toString()코드를 자동 추가
```java
 pom.xml <dependency> 밑에서 ctrl+space를 누른후 [edit starters..]를 더블 클릭 하여
 'Lombok'체크
 + java -jar lombok-1.18.10.jar 하여 STS설치 위치를 지정한 후 설치
 + eclipse 재기동
```
