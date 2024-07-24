---
aliases:
  - calculus
  - 적분과 미분
category:
  - 수학
related_concepts:
  - 미분
  - 적분
  - 극한
  - 연속성
  - 함수
tags:
  - 수학
  - 해석학
  - 뉴턴
  - 라이프니츠
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
# 미적분

## 정의
미적분(微積分, Calculus)은 함수의 변화율과 누적값을 다루는 수학의 한 분야다. 주로 미분과 적분으로 구성되며, 물리학, 공학, 경제학 등 다양한 분야에서 광범위하게 응용된다.

## 핵심 원리
1. 미분(Differentiation): 함수의 순간 변화율을 구하는 과정
2. 적분(Integration): 함수의 누적값을 구하는 과정
3. 미분과 적분의 관계: 미적분의 기본 정리에 의해 서로 역연산 관계

## 상세 설명

### 미분
미분은 함수의 순간 변화율을 구하는 과정이다. 주어진 함수 $f(x)$에 대해, 그 도함수 $f'(x)$는 다음과 같이 정의된다:

$$f'(x) = \lim_{h \to 0} \frac{f(x+h) - f(x)}{h}$$

이는 함수의 기울기를 나타내며, 물리에서는 속도나 가속도를 계산하는 데 사용된다.

### 적분
적분은 함수의 누적값을 구하는 과정이다. 정적분은 다음과 같이 정의된다:

$$\int_a^b f(x) dx = \lim_{n \to \infty} \sum_{i=1}^n f(x_i) \Delta x$$

여기서 $[a,b]$는 적분 구간이며, $\Delta x = \frac{b-a}{n}$이다.

### 미적분의 기본 정리
미적분의 기본 정리는 미분과 적분이 서로 역연산 관계임을 보여준다:

$$\frac{d}{dx} \int_a^x f(t) dt = f(x)$$

## 적용 예시
- 물리학: 속도와 거리 계산
- 공학: 최적화 문제 해결
- 경제학: 한계 비용과 총 비용 분석

## 역사적 배경
미적분은 17세기에 [[Isaac Newton|아이작 뉴턴]]과 고트프리트 라이프니츠에 의해 독립적으로 발전되었다. 두 수학자의 접근 방식은 달랐지만, 결과적으로 같은 개념에 도달했다.

## 실험적 증거
미적분의 원리는 물리 현상을 정확히 설명하는 데 성공했으며, 이는 미적분의 유효성을 입증한다. 예를 들어, 케플러의 행성 운동 법칙은 뉴턴의 미적분을 통해 더 정확히 설명될 수 있었다.

## 한계와 예외
미적분은 연속함수에 대해 가장 잘 작동하며, 불연속 함수나 특이점이 있는 경우 주의가 필요하다.

## 관련 개념
- [[극한]]
- [[연속성]]
- [[테일러 급수]]
- [[편미분]]

## 응용 분야
- 물리학
- 공학
- 경제학
- 통계학
- 컴퓨터 그래픽스


## 참고문헌
1. Stewart, J. (2015). Calculus: Early Transcendentals. Cengage Learning.
2. Apostol, T. M. (1967). Calculus, Vol. 1: One-Variable Calculus with an Introduction to Linear Algebra. Wiley.
3. Spivak, M. (2006). Calculus. Cambridge University Press.

