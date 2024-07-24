---
aliases:
  - 플럭스
  - 유량
  - 선속
category:
  - 물리학
  - 수학
related_concepts:
  - 벡터장
  - 발산
  - 가우스 정리
  - 전기장
tags:
  - 벡터해석
  - 전자기학
  - 유체역학
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
# 플럭스 (Flux)
## 정의
플럭스(Flux), 혹은 선속은 벡터장을 통과하는 양을 나타내는 물리량이다. 일반적으로 단위 면적당 흐르는 양으로 정의된다.

## 수학적 표현
벡터장 $\mathbf{F}$에 대한 면 $S$를 통과하는 플럭스:

$$\Phi = \iint_S \mathbf{F} \cdot d\mathbf{A}$$

여기서 $d\mathbf{A}$는 면적 요소 벡터다.

## 핵심 개념
1. 벡터장의 '세기'를 측정한다.
2. 스칼라량으로, 방향은 없고 크기만 있다.
3. 양수, 음수, 또는 0이 될 수 있다.

## 물리적 의미
- 전기장: 전하의 흐름
- 자기장: 자기력선의 밀도
- 유체역학: 유체의 흐름량


## 관련 정리
- 가우스 발산 정리: 닫힌 면을 통과하는 플럭스는 그 내부 발산의 체적 적분과 같다.

$$\oint_S \mathbf{F} \cdot d\mathbf{A} = \iiint_V \nabla \cdot \mathbf{F} \, dV$$

## 예시
1. 전기 플럭스: $\Phi_E = \oint \mathbf{E} \cdot d\mathbf{A} = \frac{Q}{\epsilon_0}$
2. 자기 플럭스: $\Phi_B = \oint \mathbf{B} \cdot d\mathbf{A} = 0$

## 주의점
1. 플럭스는 면적에 의존한다.
2. 벡터장과 면의 상대적 방향이 중요하다.

## 참고문헌
1. Griffiths, D. J. (2017). Introduction to Electrodynamics. Cambridge University Press.
2. Feynman, R. P., Leighton, R. B., & Sands, M. (2011). The Feynman Lectures on Physics, Vol. II. Basic Books.