---
layout: post
title: 170320 JAVA授業
---

## @Override 주석
자바 컴파일러는 @Override 주석이 사용되어 메소드가 선언되면 상위 클래스의 메소드와 정확하게 일치하는지 검사하여 일치하지 않은 경우에는 컴파일 오류를 발생시킨다.

ex) 오버라이딩 되는 메서드의 이름을 잘못 적은 경우
```java
class AA {
  public void show(String str) {
  
  }
}

class BB extends AA {
  @Override
  pulbic void shaw(String str) {  //ERROR!
  
  }
}
