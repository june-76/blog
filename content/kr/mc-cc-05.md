---
title: "TIL(Today I Learn) Day 5"
date: "2024-10-17"
description: ""
category: "learning-notes"
---

### 오늘의 책 읽기: 추천사 ~ 4장. 주석

![](/images/GZnIkgKacAAt67Q.jpg)

### 기억에 남는, 기억하고 싶은 내용

- 주석이 필요한 상황에 처하면 곰곰이 생각하기 바란다. 상황을 역전해 코드로 의도를 표현할 방법은 없을까?(p.68 line12)
- 다음 코드 예제 두 개를 살펴보자. 어느 쪽이 더 나은가?(p.70 line3)
    ```java
    // 직원에게 복지 혜택을 받을 자격이 있는지 검사한다.
    if ((employess.flags & HOURLY_FLAG) && (employee.age > 65))
    ```
    ```java
    if (employee.isEligibleForFullBenefits())
    ```
- 특별한 이유 없이 의무감으로 혹은 프로세스에서 하라고 하니까 마지못해 주석을 단다면 전적으로 시간낭비다. 주석을 달기로 결정했다면 충분한 시간을 들여 최고의 주석을 달도록 노력한다.(p.76 line2)
- **목록 4-2 ContainerBase.java(톰캣) (p.77~p.79)**
- 주석을 달아야 한다면 근처에 있는 코드만 기술하라. 코드 일부에 주석을 달면서 시스템의 전반적인 정보를 기술하지 마라.(p.88 line2)

### 읽은 감상

- 주석은 조직에서 정한 규칙에 따라 작성하는 경우가 많았다. 예를 들면 각 소스 파일의 최상단에 조항이나 규정 등을 기재하는 것이다. 그 외에는 주석을 잘 사용하지 않았다. 단순히 주석을 작성하면 전체 코드의 줄 수가 늘게 되고, 읽어야 하는 코드가 많아지니 부담스러울 수 있다는 생각이었다. 깔끔해보이기도 하고. 본 서적에서 제시하는 ‘코드 자체가 주석 없이도 이해될 수 있어야 한다’는 철학에 따른 것은 아니었다. ‘주석을 없애자’는 의미 없는 목적 말고, ‘주석이 없어도 되는’ 코드를 작성할 수 있도록 신경을 써보자.
- 예외적으로 TODO 주석은 잘 사용하는 편이다. 아무리 메신저, jira 등의 협업도구를 사용한다 하더라도 코드 바로 근처에 직접 작성하는 것이 가장 효과적이었다.

### 더 알아보고 싶은 것들

- javadoc
    - Generates HTML pages of API documentation from Java source files.
        [javadoc](https://docs.oracle.com/javase/8/docs/technotes/tools/windows/javadoc.html)

#노개북 #노마드코더 #개발자북클럽
