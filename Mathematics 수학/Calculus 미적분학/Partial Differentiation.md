---
aliases:
  - partial differentiation
  - 부분 미분
category:
  - 수학
  - 해석학
related_concepts:
  - 전미분
  - 다변수 함수
  - 그라디언트
  - 방향미분
tags:
  - 수학
  - 해석학
  - 벡터
  - 해석
  - 열역학
  - 미적분학
---

```table-of-contents
title: 
style: nestedList # TOC style (nestedList|nestedOrderedList|inlineFirstLevel)
minLevel: 0 # Include headings from the specified level
maxLevel: 0 # Include headings up to the specified level
includeLinks: true # Make headings clickable
debugInConsole: false # Print debug info in Obsidian console
```
# 편미분 (Partial Differentiation)

## 정의
편미분(偏微分, Partial differentiation)은 다변수 함수에서 하나의 변수에 대해서만 미분을 수행하는 연산이다. 이때 다른 변수들은 상수로 취급한다.

## 핵심 원리
1. 한 변수에 대해서만 미분하고 나머지는 상수 취급
2. 각 변수별로 함수의 변화율을 독립적으로 측정
3. 다변수 함수의 국소적 변화를 분석하는 도구

## 수학적 표현
함수 $f(x, y)$의 $x$에 대한 편미분:

$$\frac{\partial f}{\partial x} = \lim_{h \to 0} \frac{f(x+h, y) - f(x, y)}{h}$$

## 표기법
1. 리이브니츠 표기법: $\frac{\partial f}{\partial x}$, $\frac{\partial f}{\partial y}$
2. 라그랑주 표기법: $f_x$, $f_y$

## 계산 방법
1. 미분하려는 변수 외의 모든 변수를 상수 취급하고, 
2. 그 이후에는 일반적인 미분 규칙을 동일하게 적용

예: $f(x,y) = x^2y + xy^3$의 편미분
- $\frac{\partial f}{\partial x} = 2xy + y^3$
- $\frac{\partial f}{\partial y} = x^2 + 3xy^2$

## 고차 편미분
같은 변수로 여러 번 편미분:
$$\frac{\partial^2 f}{\partial x^2} = \frac{\partial}{\partial x}\left(\frac{\partial f}{\partial x}\right)$$

## 혼합 편미분
서로 다른 변수로 연속 편미분:
$$\frac{\partial^2 f}{\partial x \partial y} = \frac{\partial}{\partial x}\left(\frac{\partial f}{\partial y}\right)$$

중요: 연속인 혼합 편미분은 순서 교환 가능 (클레로의 정리)
$$\frac{\partial^2 f}{\partial x \partial y} = \frac{\partial^2 f}{\partial y \partial x}$$

## 응용 분야
1. 물리학: 열역학, 전자기학, 유체역학
2. 공학: 최적화 문제, 제어 이론
3. 경제학: 한계 분석, 탄력성 계산
4. 기계학습: 신경망의 오차 역전파 알고리즘

## 기하학적 해석
편미분은 다변수 함수의 특정 방향으로의 기울기를 나타낸다. 3차원 그래프에서 $x$나 $y$ 축과 평행한 평면으로 자른 단면의 기울기와 같다.

## 중요한 성질
1. 선형성: $\frac{\partial}{\partial x}(af + bg) = a\frac{\partial f}{\partial x} + b\frac{\partial f}{\partial x}$
2. 곱의 법칙: $\frac{\partial}{\partial x}(fg) = f\frac{\partial g}{\partial x} + g\frac{\partial f}{\partial x}$
3. 연쇄 법칙: $\frac{\partial f}{\partial x} = \frac{\partial f}{\partial u}\frac{\partial u}{\partial x} + \frac{\partial f}{\partial v}\frac{\partial v}{\partial x}$

## 역사적 배경
편미분의 개념은 18세기에 오일러와 라그랑주에 의해 발전되었다. 이들은 다변수 함수의 해석에 이 개념을 도입했다.

## 한계와 주의점
1. 불연속점에서는 편미분이 존재하지 않을 수 있다.
2. 모든 편미분이 존재해도 함수가 미분가능하지 않을 수 있다.
3. 편미분의 연속성이 함수의 연속성을 보장하지 않는다.

## 관련 개념
- [[전미분]]
- [[그라디언트]]
- [[방향미분]]
- [[테일러 급수]]

## 학습 팁
1. 단변수 미분을 완벽히 이해한 후 편미분을 학습한다.
2. 다양한 예제를 통해 여러 변수에 대한 편미분을 연습한다.
3. 편미분의 기하학적 의미를 이해하려 노력한다.
4. 실제 문제에 적용해보며 개념을 확고히 한다.

## 연습 문제
1. $f(x,y) = x^3 + y^3 + 3xy$의 모든 1차, 2차 편미분을 구하시오.
2. $f(x,y,z) = xe^{yz}$의 $\frac{\partial^2 f}{\partial y \partial z}$를 구하시오.

## 참고문헌
1. Stewart, J. (2015). Calculus: Early Transcendentals. Cengage Learning.
2. Apostol, T. M. (1969). Calculus, Vol. 2: Multi-Variable Calculus and Linear Algebra with Applications. Wiley.
3. Marsden, J. E., & Tromba, A. J. (2011). Vector Calculus. W. H. Freeman.

## 추가 노트
편미분은 다변수 해석학의 기초가 되는 개념으로, 벡터 해석과 텐서 해석으로 확장된다. 특히 물리학에서는 장(field) 이론을 이해하는 데 필수적인 도구다. 또한 최적화 문제에서 그라디언트 하강법의 기초가 되어 현대 기계학습 알고리즘에도 널리 사용된다.