---
aliases:
  - Dirac notation
  - 브라-켓 표기법
  - bra-ket notation
category:
  - 양자역학
  - 선형대수학
related_concepts:
  - 힐베르트 공간
  - 양자상태
  - 내적
  - 연산자
tags:
  - 양자역학
  - 표기법
  - 선형대수학
  - 물리
  - 수학
---

```table-of-contents
title: 
style: nestedList # TOC style (nestedList|nestedOrderedList|inlineFirstLevel)
minLevel: 0 # Include headings from the specified level
maxLevel: 0 # Include headings up to the specified level
includeLinks: true # Make headings clickable
debugInConsole: false # Print debug info in Obsidian console
```
# 디랙 표기법

## 정의

디랙 표기법은 폴 디랙이 도입한 양자역학에서 사용되는 수학적 표기법이다. 이 표기법은 벡터와 선형 연산자를 간결하고 일관된 방식으로 표현한다. 주요 요소는 다음과 같다:

- 켓(ket) 벡터: $|\psi\rangle$
- 브라(bra) 벡터: $\langle\psi|$
- 내적: $\langle\phi|\psi\rangle$
- 외적: $|\psi\rangle\langle\phi|$

## 중요 성질

1. 선형성: $|\alpha\psi + \beta\phi\rangle = \alpha|\psi\rangle + \beta|\phi\rangle$
2. 내적의 에르미트 성질: $\langle\phi|\psi\rangle = \langle\psi|\phi\rangle^*$
3. 완전성 관계: $\sum_i |i\rangle\langle i| = 1$
4. 연산자의 표현: $\hat{A} = \sum_{i,j} |i\rangle\langle i|\hat{A}|j\rangle\langle j|$

## 주요 정리

1. 슈미트 분해 정리
   증명: 임의의 상태 $|\psi\rangle$는 $|\psi\rangle = \sum_i c_i |i\rangle$로 표현할 수 있다.

2. 스펙트럼 정리
   증명: 에르미트 연산자 $\hat{A}$는 $\hat{A} = \sum_i a_i |i\rangle\langle i|$로 표현할 수 있다.

## 응용

- 양자역학의 상태 벡터 표현
- 양자 연산자의 표현
- 양자 측정 이론
- 양자 정보 이론
- 양자 계산

## 관련 개념

- 힐베르트 공간
- 선형 연산자
- 고유값과 고유벡터
- 에르미트 연산자
- 유니터리 연산자

## 예제

1. 내적 계산
   해설: $\langle\phi|\psi\rangle = \sum_i \phi_i^* \psi_i$

2. 연산자의 기댓값
   해설: $\langle\hat{A}\rangle = \langle\psi|\hat{A}|\psi\rangle$

## 역사적 배경

디랙 표기법은 1930년대 폴 디랙에 의해 도입되었다. 이 표기법은 양자역학의 수학적 구조를 간결하고 명확하게 표현할 수 있어 빠르게 표준이 되었다.

## 시각화

[브라와 켓 벡터의 기하학적 해석 다이어그램]
[힐베르트 공간에서의 벡터 표현]

## 계산 방법

1. 내적 계산: $\langle\phi|\psi\rangle = \sum_i \phi_i^* \psi_i$
2. 연산자 적용: $\hat{A}|\psi\rangle = \sum_i a_i |i\rangle\langle i|\psi\rangle$
3. 행렬 요소 계산: $\langle i|\hat{A}|j\rangle$

## 주의사항

- 브라와 켓의 순서에 주의해야 한다.
- 복소수 공액 관계를 항상 고려해야 한다.
- 무한차원 힐베르트 공간에서는 수렴성에 주의해야 한다.

## 참고 문헌

1. Dirac, P. A. M. (1939). The Principles of Quantum Mechanics. Oxford University Press.
2. Sakurai, J. J., & Napolitano, J. (2017). Modern Quantum Mechanics. Cambridge University Press.
3. Nielsen, M. A., & Chuang, I. L. (2010). Quantum Computation and Quantum Information. Cambridge University Press.

