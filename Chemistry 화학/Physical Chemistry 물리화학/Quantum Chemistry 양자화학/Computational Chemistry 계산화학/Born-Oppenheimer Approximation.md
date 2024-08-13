---
aliases:
  - BO 근사
  - 보른-오펜하이머 근사
category:
  - 양자화학
  - 계산화학
related_concepts:
  - 단열 근사
  - 전자-핵 분리
  - 포텐셜 에너지 표면
tags:
  - 양자역학
  - 분자
  - 구조
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
# 보른-오펜하이머 근사 (Born-Oppenheimer Approximation)

## 정의 및 개요

보른-오펜하이머 근사는 분자의 전자와 핵의 운동을 분리하여 다루는 양자역학적 근사 방법이다. 핵의 질량이 전자에 비해 매우 크기 때문에 핵이 정지해 있다고 가정하고 전자의 운동만을 고려한다. 이 근사법은 1927년 막스 보른과 로버트 오펜하이머에 의해 제안되었으며, 분자 양자역학의 기초가 되었다.

## 핵심 원리
1. 핵과 전자의 질량 차이: 핵은 전자보다 수천 배 이상 무겁다.
2. 시간 척도 분리: 전자의 운동은 핵의 운동보다 훨씬 빠르다.
3. 전자-핵 분리: 전체 파동함수를 전자와 핵의 파동함수의 곱으로 근사한다.

## 수학적 표현
보른-오펜하이머 근사에서 전체 파동함수 $\Psi$ 는 다음과 같이 표현된다:

$$\Psi(r,R) \approx \psi_e(r;R) \chi_n(R)$$

여기서 $r$은 전자 좌표, $R$은 핵 좌표, $\psi_e$는 전자 파동함수, $\chi_n$은 핵 파동함수이다.

## 적용 예시
- 분자 구조 계산
- 포텐셜 에너지 표면 구성
- 화학 반응 경로 분석

## 관련 개념
- [[단열 근사]]
- [[포텐셜 에너지 표면]]
- [[전자-핵 분리]]

## 응용 분야
- 양자화학 계산
- 분자 분광학
- 반응 동력학 시뮬레이션

## 여담
- 보른-오펜하이머 근사는 양자화학 계산의 기본이 되는 매우 중요한 개념이다. 그러나 매우 가벼운 원자(예: 수소)가 포함된 시스템에서는 정확도가 떨어질 수 있으며, 전자 상태 간 전이가 중요한 경우(예: 비단열 과정)에는 적용이 어렵다. 이 근사법의 한계를 이해하고 적절히 적용하는 것이 중요하다.

- 학습 시 고전역학에서의 질점 운동과 비교하며 이해하는 것이 도움이 된다. 전자와 핵의 질량 차이가 왜 중요한지 생각해보고, 간단한 분자(예: H₂)에 대해 직접 계산을 수행해보는 것도 좋은 학습 방법이다.

## 참고문헌
1. Born, M.; Oppenheimer, R. (1927). "Zur Quantentheorie der Molekeln". Annalen der Physik. 389 (20): 457–484.
2. Levine, I. N. (2000). Quantum Chemistry (5th ed.). Prentice Hall.
3. Szabo, A.; Ostlund, N. S. (1996). Modern Quantum Chemistry. Dover Publications.