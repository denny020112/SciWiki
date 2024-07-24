---
aliases:
  - 전미분
  - 전체 미분
  - 완전 미분
category:
  - 수학
  - 해석학
related_concepts:
  - 편미분
  - 다변수 함수
  - 연쇄 법칙
  - 그라디언트
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
# 전미분 (Total Differential)

## 정의
전미분(全微分, Total differential)은 다변수 함수에서 모든 변수의 미소 변화에 따른 함수값의 전체 변화를 나타내는 개념이다. 각 변수의 편미분을 이용하여 표현된다.

## 핵심 원리
1. 각 변수의 미소 변화에 따른 함수값의 변화를 모두 합한다.
2. 각 변수의 변화에 대한 기여도는 해당 변수에 대한 편미분으로 표현된다.
3. 전미분은 함수의 근사적 선형화를 제공한다.

## 상세 설명

### 수학적 표현
2변수 함수 $f(x,y)$의 전미분은 다음과 같이 표현된다:

$$df = \frac{\partial f}{\partial x}dx + \frac{\partial f}{\partial y}dy$$

여기서 $dx$와 $dy$는 각각 $x$와 $y$의 미소 변화량을 나타낸다.

n변수 함수 $f(x_1, x_2, ..., x_n)$의 경우:

$$df = \sum_{i=1}^n \frac{\partial f}{\partial x_i}dx_i$$

### 기하학적 의미
전미분은 다변수 함수의 접평면(tangent plane)을 나타낸다. 즉, 함수의 로컬 선형 근사(local linear approximation)를 제공한다.

### 전미분과 함수의 변화량
함수 $f(x,y)$에서 점 $(x,y)$에서 $(x+\Delta x, y+\Delta y)$로의 변화에 대해:

$$\Delta f \approx df = \frac{\partial f}{\partial x}\Delta x + \frac{\partial f}{\partial y}\Delta y$$

이는 함수의 변화를 1차(선형) 항까지 근사한 것이다.

### 전미분의 정확성
함수가 연속이고 편미분이 연속이면, 전미분은 함수의 실제 변화를 정확히 나타낸다:

$$\lim_{\Delta x, \Delta y \to 0} \frac{\Delta f - df}{\sqrt{(\Delta x)^2 + (\Delta y)^2}} = 0$$

## 적용 예시
1. 열역학: 상태 함수의 변화를 표현하는 데 사용
   예: 내부 에너지 $U(S,V)$의 전미분
   $$dU = T dS - P dV$$

2. 오차 분석: 측정값의 불확실성 전파를 계산하는 데 활용

3. 최적화: 경사 하강법(gradient descent)에서 함수의 로컬 근사에 사용

## 역사적 배경
전미분의 개념은 18세기 말에서 19세기 초에 걸쳐 발전되었다. 오일러, 라그랑주, 코시 등이 이 개념의 발전에 기여했다.

## 실험적 증거
전미분은 많은 물리 법칙을 간결하게 표현하는 데 사용된다. 예를 들어, 열역학 제1법칙은 전미분 형태로 표현될 수 있다.

## 한계와 예외
1. 불연속점에서는 전미분이 정의되지 않는다.
2. 편미분이 연속이 아닌 경우, 전미분의 정확성이 보장되지 않는다.

## 관련 개념
- [[편미분]]
- [[그라디언트]]
- [[연쇄 법칙]]
- [[접평면]]

## 응용 분야
1. 물리학: 열역학, 전자기학, 유체역학
2. 공학: 제어 이론, 신호 처리
3. 경제학: 한계 분석, 효용 이론
4. 금융공학: 리스크 관리, 포트폴리오 최적화

## 최근 연구 동향
1. 기계학습: 신경망의 역전파 알고리즘에서 전미분 개념 활용
2. 복잡계 과학: 다변수 시스템의 동역학 분석에 적용

## 학습 팁
1. 편미분을 철저히 이해한 후 전미분 개념을 학습한다.
2. 전미분의 기하학적 의미를 시각화하려 노력한다.
3. 실제 물리 문제에 적용해보며 개념을 확고히 한다.

## 연습 문제
1. $f(x,y) = x^2y + xy^3$의 전미분을 구하시오.
2. $z = x^2 + y^2$에서 점 (1,1)에서의 접평면 방정식을 전미분을 이용하여 구하시오.

## 참고문헌
1. Courant, R., & John, F. (1989). Introduction to Calculus and Analysis. Springer.
2. Spivak, M. (1998). Calculus on Manifolds. Westview Press.
3. Marsden, J. E., & Tromba, A. J. (2011). Vector Calculus. W. H. Freeman.

## 추가 노트
전미분은 다변수 함수의 변화를 이해하는 핵심 도구로, 물리학과 공학에서 광범위하게 사용된다. 특히 열역학에서는 상태 함수의 변화를 기술하는 데 필수적이며, 이를 통해 복잡한 시스템의 거동을 이해할 수 있다. 또한 최적화 문제에서 함수의 로컬 동작을 분석하는 데 중요한 역할을 한다.