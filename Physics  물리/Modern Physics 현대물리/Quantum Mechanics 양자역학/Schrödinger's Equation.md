---
aliases:
  - Schrödinger equation
  - 파동 방정식
category:
  - 양자역학
  - 물리화학
related_concepts:
  - 양자역학
  - 파동함수
  - 해밀토니안
  - 고유값 문제
tags:
  - 양자역학
  - 파동함수
  - 미분방정식
  - 물리화학
  - 화학
  - 수학
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
# 슈뢰딩거 방정식

## 정의

슈뢰딩거 방정식은 양자역학의 기본 방정식으로, 입자의 파동함수 $\psi$의 시간 발전을 기술한다. 시간 의존 슈뢰딩거 방정식은 다음과 같이 정의된다:

$$ i\hbar \frac{\partial}{\partial t} \psi(\mathbf{r},t) = \hat{H} \psi(\mathbf{r},t) $$

여기서 $i$는 허수 단위, $\hbar$는 축약 플랑크 상수, $\hat{H}$는 해밀토니안 연산자이다.

## 중요 성질

1. 선형성: 슈뢰딩거 방정식은 선형 미분방정식이다.
2. 확률 해석: $|\psi|^2$는 입자의 확률 밀도를 나타낸다.
3. 고유값 문제: 시간 독립 슈뢰딩거 방정식은 고유값 문제의 형태를 가진다.
4. 파동-입자 이중성: 입자의 파동적 성질을 기술한다.

## 주요 정리

1. 에너지 고유값 정리
   증명: 시간 독립 슈뢰딩거 방정식 $\hat{H}\psi = E\psi$의 해는 시스템의 정상 상태를 나타낸다.

2. 기대값 정리
   증명: 관측량 $A$의 기대값은 $\langle A \rangle = \int \psi^* \hat{A} \psi d\tau$로 주어진다.

3. 시간 발전 연산자
   증명: $\psi(t) = e^{-i\hat{H}t/\hbar} \psi(0)$

## 응용

- 원자 및 분자 구조 계산
- 화학 결합 이론
- 분광학 
- 고체 물리학
- 양자 화학

## 관련 개념

- 하이젠베르크의 불확정성 원리
- 파울리 배타 원리
- 변분 원리
- 섭동 이론

## 예제

1. 무한 퍼텐셜 우물 문제
   해설: 1차원 무한 퍼텐셜 우물에서의 입자의 파동함수와 에너지 준위를 구한다.

2. 수소 원자 문제
   해설: 수소 원자의 전자 파동함수와 에너지 준위를 계산한다.

## 역사적 배경

1925년 에르빈 슈뢰딩거에 의해 제안되었다. 그는 드브로이의 물질파 개념을 바탕으로 이 방정식을 유도했으며, 이는 양자역학의 발전에 핵심적인 역할을 했다.

## 시각화

[파동함수의 시간에 따른 변화를 나타내는 애니메이션]
[수소 원자의 전자 궤도함수 그림]

## 계산 방법

1. 해석적 방법: 단순한 시스템에 대해 정확한 해를 구한다.
2. 변분법: 복잡한 시스템의 근사해를 구한다.
3. 섭동법: 작은 변화가 있는 시스템의 해를 근사적으로 구한다.
4. 수치해석: 컴퓨터를 이용해 복잡한 시스템의 해를 구한다.

## 주의사항

- 해석해를 구할 수 있는 시스템은 제한적이다.
- 다체계 문제는 매우 복잡하여 근사법이 필요하다.
- 상대론적 효과를 고려하지 않는다 (비상대론적 방정식).

## 참고 문헌

1. Griffiths, D. J. (2018). Introduction to quantum mechanics. Cambridge University Press.
2. McQuarrie, D. A. (2008). Quantum chemistry. University Science Books.
3. Levine, I. N. (2013). Quantum chemistry. Pearson.

## 추가 학습 자료

- MIT OpenCourseWare: Quantum Physics I
- Coursera: Quantum Mechanics for Scientists and Engineers
- YouTube: 3Blue1Brown의 양자역학 시리즈