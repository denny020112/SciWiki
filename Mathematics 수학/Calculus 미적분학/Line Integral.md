---
aliases:
  - 경로 적분
  - 선적분
category:
  - 미적분학
  - 벡터 해석
related_concepts:
  - 그린 정리
  - 스토크스 정리
  - 보존장
tags:
  - 적분
  - 벡터장
  - 경로
  - 수학
  - 미적분학
  - 물리
---

```table-of-contents
title: 
style: nestedList # TOC style (nestedList|nestedOrderedList|inlineFirstLevel)
minLevel: 0 # Include headings from the specified level
maxLevel: 0 # Include headings up to the specified level
includeLinks: true # Make headings clickable
debugInConsole: false # Print debug info in Obsidian console
```
# 선적분 (line integral)

## 정의
선적분은 곡선에 있는 모든 점에 대해 함수나 벡터장의 적분을 구하는 것이다. 
장(field)에 대한 선적분은 스칼라장이나 벡터장을 특정 경로 곡선 C를 따라 적분하는 것을 의미한다.

## 핵심 원리
1. 곡선을 따라 적분한다
2. 스칼라장과 벡터장 모두에 대해 정의된다
3. 경로 의존성이 있을 수 있다

## 상세 설명

### 스칼라장의 선적분
![[scalar field line integral 2D.png|450]]
![[scalar field line integral 3D.png|450]]
스칼라 함수 $f(x,y)$의 선적분은 다음과 같이 정의된다:

$$ \int_C f(x,y) ds = \int_a^b f(x(t),y(t)) \sqrt{\left(\frac{dx}{dt}\right)^2 + \left(\frac{dy}{dt}\right)^2} dt $$

여기서 $(x(t),y(t))$는 곡선 C의 매개변수 표현이며, $a \leq t \leq b$이다.

### 벡터장의 선적분

![[vector field line integral.png|500]]
벡터장 $\mathbf{F}(x,y) = P(x,y)\mathbf{i} + Q(x,y)\mathbf{j}$의 선적분은 다음과 같이 정의된다:

$$ \int_C \mathbf{F} \cdot d\mathbf{r} = \int_a^b [P(x(t),y(t))\frac{dx}{dt} + Q(x(t),y(t))\frac{dy}{dt}] dt $$

## 적용 예시
- 물리학: 일의 계산. 
	- 물리 실험에서 일이나 전위차를 측정하여 선적분의 결과를 검증할 수 있다.
- 전자기학: 전위차 계산
- 유체역학: 유량 계산
## 관련 개념
- [[그린 정리]]: 폐곡선에서의 선적분은 그린 정리를 통해 영역 적분으로 변환할 수 있다.
- [[스토크스 정리]]
- [[보존장]]


## 참고문헌
1. Stewart, J. (2015). Calculus: Early Transcendentals. Cengage Learning.
2. Kreyszig, E. (2011). Advanced Engineering Mathematics. John Wiley & Sons.

