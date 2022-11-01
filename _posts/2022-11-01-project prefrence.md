---
layout: single
title: "프로젝트환경설정"
---


### #Spring initializr

![Untitled](%E1%84%91%E1%85%B3%E1%84%85%E1%85%A9%E1%84%8C%E1%85%A6%E1%86%A8%E1%84%90%E1%85%B3%20%E1%84%92%E1%85%AA%E1%86%AB%E1%84%80%E1%85%A7%E1%86%BC%E1%84%89%E1%85%A5%E1%86%AF%E1%84%8C%E1%85%A5%E1%86%BC%20d59a3496ee184a8480c5ed5cf026cabf/Untitled.png)


**Gradle project vs Maven project**

버전을 설정하고 라이브러리를 땡겨옴


**Dependencies**

어떤 라이브러리를 땡겨쓸 것인지 선택

**Thymeleaf**


html을 만들어주는 템플릿 엔진

**.idea**

인텔리제이가 사용하는 설정파일


**main vs test**

main → java, resource

test → test 코드들과 관련된 소스들이 존재


### #라이브러리

Gradle은 의존 관계가 있는 라이브러리를 함께 다운로드 한다.


**스프링부트 라이브러리**

- spring-boot-starter-web
    - spring-boot-starter-tomcat : 톰캣 (웹서버)
    - spring-webmvc : 스프링 웹 MVC
- spring-boot-starter-thymeleaf : 타임리프 템플릿 엔진 (View)
- spring-boot-starter (공통) : 스프링 부트 + 스프링 코어 + 로깅
    - spring-boot
        - spring-core
    - spring-boot-starter-logging
        - logback, slf4j
        
        
**테스트 라이브러리**

- spring-boot-starter-test
    - junit : 테스트 프레임워크
    - mockito : 목 라이브러리
    - assertj : 테스트 코드를 좀 더 편하게 작성하게 도와주는 라이브러리
    - spring-test : 스프링 통합 테스트 지원
    

**External Libraries**

땡겨오는 라이브러리들 (tomcat 내장해서 올라옴)


**logging**

현업에서는 System.out.println으로 출력X ⇒ log로 출력O

log로 출력하면 심각한 에러들을 따로 모아서 보거나 log 파일이 관리됨

slf4j → 인터페이스, logback → 실제 로그를 어떤 구현체로 출력할 것인지 선택
