---
layout: post
title: Adapter Pattern Facade Pattern
tags: [DesignPattern]
---

### Adapter Pattern 어댑터 패턴
* 클래스의 인터페이스를 클라이언트가 원하는 대로 변경
* 어댑터는 호환 불가능한 인터페이스 때문에 협력할 수 없는 클래스 들을 협력할 수 있게함.
* Wrapper 로도 불림
* 레거시 시스템을 원하는 인터페이스로 사용 가능케 한다.
* 여기서 레거시 시스템(legacy system) 이란?   
* 레거시 시스템(legacy system) : 프로그래밍 언어, 플랫폼 그리고 기술 등에 있어, 과거로 부터 물려 내려온 것

client와 연결된 어댑터는 레거시 시스템이 제공하는 api로 내용을 바꾼다.

* 클래스 어댑터 

### Facade Pattern 퍼싸드 패턴
* 시스템을 특정한 방법으로 사용
* 복잡한 내용을 쉽게 사용할만한 인터페이스를 주고싶다면??
* 서브시스템 사용을 간소화 시킬 수 있다.
* 클라이언트 객체가 다룰 객체의 수를 줄여준다.
* 새로운 기능 추가, 확장
* 캡슐화
<img src = "https://springframework.guru/wp-content/uploads/2015/07/Facade02.png"/>
https://springframework.guru/

### 어댑터 VS 퍼싸드
어댑터 패턴은 클라이언트가 사용하고자 하는 다른 인터페이스로 기존의 인터페이스를 조정하는데에 있고
퍼사드 패턴의 목적은 서브시스템과 상호작용 복잡도를 낮추는데에 있다.


