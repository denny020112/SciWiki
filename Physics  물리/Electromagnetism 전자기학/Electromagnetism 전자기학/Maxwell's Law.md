---
aliases:
  - Maxwell's equations
  - 맥스웰 방정식
category:
  - 전자기학
  - 물리학
related_concepts:
  - 전기장
  - 자기장
  - 전자기파
  - 패러데이 법칙
  - 앙페르 법칙
tags:
  - 전자기학
  - 고전물리학
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
# 맥스웰의 법칙 (Maxwell's Equations)

## 개요
맥스웰의 법칙은 전기장과 자기장의 관계를 설명하는 4개의 편미분 방정식으로, 전자기학의 근간을 이루는 가장 중요한 법칙이다. 제임스 클러크 맥스웰(James Clerk Maxwell)이 1861년부터 1865년 사이에 발표한 논문에서 처음 제시되었다.

## 역사적 배경

맥스웰의 법칙은 19세기 초반부터 중반까지 발전된 전기와 자기에 대한 연구를 종합한 결과물이다. 주요 선행 연구는 다음과 같다:

1. 쿨롱의 법칙 (1785): 전하 사이의 정전기력 설명
2. 앙페르의 법칙 (1820): 전류와 자기장의 관계 설명
3. 패러데이의 전자기 유도 법칙 (1831): 자기장 변화에 의한 전기장 유도 설명

맥스웰은 이러한 선행 연구들을 종합하고, 특히 '변위 전류' 개념을 도입하여 전자기 이론을 완성했다.

## 맥스웰 방정식

맥스웰의 법칙은 다음 4개의 방정식으로 구성된다:

1. 가우스의 전기 법칙:

   $$ \nabla \cdot \mathbf{E} = \frac{\rho}{\epsilon_0} $$

2. 가우스의 자기 법칙:

   $$ \nabla \cdot \mathbf{B} = 0 $$

3. 패러데이의 전자기 유도 법칙:

   $$ \nabla \times \mathbf{E} = -\frac{\partial \mathbf{B}}{\partial t} $$

4. 앙페르-맥스웰 법칙:

   $$ \nabla \times \mathbf{B} = \mu_0 \mathbf{J} + \mu_0 \epsilon_0 \frac{\partial \mathbf{E}}{\partial t} $$

여기서:
- $\mathbf{E}$: 전기장
- $\mathbf{B}$: 자기장
- $\rho$: 전하 밀도
- $\mathbf{J}$: 전류 밀도
- $\epsilon_0$: 진공의 유전율
- $\mu_0$: 진공의 투자율

## 유도

맥스웰 방정식의 완전한 유도 과정은 복잡하지만, 주요 단계를 간략히 설명하면 다음과 같다:

1. 가우스의 전기 법칙: 쿨롱의 법칙을 연속 전하 분포로 확장하여 유도

2. 가우스의 자기 법칙: 자기 모노폴의 비존재성에 기반하여 유도

3. 패러데이의 전자기 유도 법칙: 패러데이의 실험 결과를 수학적으로 표현

4. 앙페르-맥스웰 법칙: 
   - 앙페르의 법칙 시작: $\nabla \times \mathbf{B} = \mu_0 \mathbf{J}$
   - 맥스웰의 변위 전류 추가: $\mu_0 \epsilon_0 \frac{\partial \mathbf{E}}{\partial t}$

특히 4번 방정식에서 맥스웰의 핵심 기여인 변위 전류 항의 도입이 중요하다. 이 항은 시간에 따라 변하는 전기장이 자기장을 유도할 수 있음을 나타내며, 전자기파의 존재를 예측하게 해주었다.

## 중요성

1. 전자기파의 예측: 맥스웰 방정식을 통해 전자기파의 존재가 이론적으로 예측되었으며, 이는 후에 헤르츠에 의해 실험적으로 확인되었다.

2. 상대성 이론과의 연관: 맥스웰 방정식은 갈릴레이 변환 하에서 불변하지 않으며, 이는 아인슈타인이 특수 상대성 이론을 발전시키는 계기가 되었다.

3. 현대 기술의 기반: 라디오, 텔레비전, 레이더, 무선 통신 등 현대의 많은 기술들이 맥스웰 방정식에 기반을 두고 있다.

## 관련 개념

- [[Electromagnetic wave]]
- [[Faraday's law of induction]]
- [[Ampère's circuital law]]
- [[Gauss's Law|가우스법칙]]

## 참고문헌

1. Maxwell, J.C. (1865). "A Dynamical Theory of the Electromagnetic Field". Philosophical Transactions of the Royal Society of London. 155: 459–512.
2. Griffiths, D.J. (2017). Introduction to Electrodynamics (4th ed.). Cambridge University Press.
3. Jackson, J.D. (1998). Classical Electrodynamics (3rd ed.). Wiley.