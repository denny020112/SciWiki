---
aliases:
  - Quantum mechanics
  - 양자물리학
  - 파동역학
category:
  - 물리학
  - 현대물리학
related_concepts:
  - 파동함수
  - 슈뢰딩거 방정식
  - 불확정성 원리
  - 중첩 원리
tags:
  - 미시세계
  - 확률론
  - 파동-입자
  - 이중성
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
# 양자역학

## 정의

양자역학은 미시세계의 물리적 현상을 설명하는 이론이다. 원자 크기 이하의 입자들의 행동을 기술하며, 고전 물리학으로는 설명할 수 없는 현상들을 다룬다. 주요 개념으로는 파동함수, 불확정성 원리, 중첩 원리 등이 있다.

## 중요 성질

1. 파동-입자 이중성: 미시 입자는 파동과 입자의 성질을 모두 가진다.
2. 불확정성 원리: 특정 물리량 쌍(예: 위치와 운동량)을 동시에 정확히 측정할 수 없다.
3. 중첩 원리: 양자 상태는 여러 가능한 상태의 중첩으로 표현될 수 있다.
4. 양자 터널링: 입자가 고전역학적으로 불가능한 장벽을 통과할 수 있다.
5. 스핀: 입자의 고유한 각운동량으로, 고전적 대응물이 없다.

## 주요 정리

1. [[Schrödinger's Equation|슈뢰딩거 방정식]]
   증명: $i\hbar\frac{\partial}{\partial t}\Psi = \hat{H}\Psi$, 여기서 $\hat{H}$는 해밀토니안 연산자이다.

2. 하이젠베르크 불확정성 원리
   증명: $\Delta x \Delta p \geq \frac{\hbar}{2}$, 여기서 $\Delta x$와 $\Delta p$는 각각 위치와 운동량의 불확정성이다.

3. 보른 규칙
   증명: $P(x) = |\Psi(x)|^2$, 여기서 $P(x)$는 위치 $x$에서 입자를 발견할 확률밀도이다.

## 응용

- 원자 및 분자 구조 이해
- 반도체 물리학
- 양자 암호학
- 양자 컴퓨팅
- 초전도체 이론
- 입자 물리학

## 관련 개념

- 파동함수
- 연산자
- 고유값과 고유함수
- 양자 중첩
- 얽힘(엔탱글먼트)
- 측정 문제

## 예제

1. 무한 퍼텐셜 우물 문제
   해설: 1차원 무한 퍼텐셜 우물에 갇힌 입자의 에너지 준위와 파동함수를 구한다.

2. 수소 원자 모델
   해설: 수소 원자의 전자 궤도와 에너지 준위를 양자역학적으로 계산한다.

## 역사적 배경

양자역학은 20세기 초 막스 플랑크, 닐스 보어, 베르너 하이젠베르크, 에르빈 슈뢰딩거 등의 과학자들에 의해 발전되었다. [[Black Body Radiation|흑체 복사]], 광전 효과, 원자 스펙트럼 등 고전 물리학으로 설명할 수 없는 현상들을 해석하기 위해 도입되었다.

## 시각화

![[Young_experiment.gif]]
[수소 원자의 전자 궤도함수 그림]
[슈뢰딩거의 고양이 사고실험 설명]

## 계산 방법

1. 슈뢰딩거 방정식 풀이: 경계 조건을 이용한 파동함수 계산
2. 연산자 방법: 기대값과 불확정성 계산
3. 섭동 이론: 복잡한 시스템의 근사 해법
4. 변분법: 기저 상태 에너지 계산

## 주의사항

- 양자역학의 해석에 대해서는 여러 견해가 존재한다 (코펜하겐 해석, 다세계 해석 등).
- 거시세계에서는 양자역학적 효과가 대부분 무시될 수 있다.
- 상대론적 효과를 고려하지 않는 비상대론적 양자역학의 한계를 인식해야 한다.

## 참고 문헌

1. Griffiths, D. J. (2018). Introduction to Quantum Mechanics. Cambridge University Press.
2. Feynman, R. P., Leighton, R. B., & Sands, M. (2011). The Feynman Lectures on Physics, Vol. III: Quantum Mechanics. Basic Books.
3. Sakurai, J. J., & Napolitano, J. (2017). Modern Quantum Mechanics. Cambridge University Press.

## 추가 학습 자료

- MIT OpenCourseWare: Quantum Physics I, II, III
- Coursera: Quantum Mechanics for Scientists and Engineers
- YouTube: PBS Space Time 채널의 양자역학 시리즈