---
aliases:
  - 슬레이터의 규칙
  - Slater's Rules
category:
  - 양자화학
  - 원자구조
  - 물리학
  - 화학
related_concepts:
  - 원자구조
  - 가우스 법칙
  - 차폐효과
tags:
  - 원자구조
  - 화학
  - 물리
  - 물리화학
---

```table-of-contents
title: 
style: nestedList # TOC style (nestedList|nestedOrderedList|inlineFirstLevel)
minLevel: 0 # Include headings from the specified level
maxLevel: 0 # Include headings up to the specified level
includeLinks: true # Make headings clickable
debugInConsole: false # Print debug info in Obsidian console
```

# 슬레이터 규칙 (Slater's Rule)

## 정의 및 개념

슬레이터 규칙은 다전자 원자에서 전자가 느끼는 유효 핵전하를 근사적으로 계산하는 방법이다. 이 규칙은 내부 전자에 의한 외부 전자의 차폐 효과를 고려한다.

## 규칙

1. 전자를 다음과 같은 그룹으로 나눈다:
   (1s) (2s,2p) (3s,3p) (3d) (4s,4p) (4d) (4f) (5s,5p) ...

2. 같은 그룹 내의 전자들은 서로를 0.35만큼 차폐한다 (단, 1s 전자는 0.30).

3. 외부 그룹의 전자들은 내부 전자를 차폐하지 않는다.

4. 내부 그룹 전자들의 차폐 효과:
   - s, p 전자에 대해: 0.85 (n-1 그룹), 1.00 (그 이전 그룹들)
   - d, f 전자에 대해: 1.00 (모든 내부 그룹)

## 수학적 표현

유효 핵전하 Z* 는 다음과 같이 계산된다:

$$Z* = Z - \sigma$$

여기서 Z는 원자 번호, σ는 차폐 상수다.

차폐 상수 σ는 다음과 같이 계산된다:

$$\sigma = \sum_{i} a_i n_i$$

여기서 a_i는 i번째 그룹의 차폐 계수, n_i는 i번째 그룹의 전자 수다.

## 적용 예시

리튬(Li, 원자번호 3)의 2s 전자에 대한 유효 핵전하:
Z* = 3 - (2 × 0.85) = 1.30

## 중요성

1. 원자의 전자 구조 이해
2. 이온화 에너지 및 전자 친화도 예측
3. 화학 결합의 특성 설명

## 한계

- 근사적인 방법으로, 정확한 값을 제공하지 않는다.
- 무거운 원자에서는 정확도가 떨어진다.
- 들뜬 상태의 원자에는 적용이 어렵다.

## 역사

- 1930년: 존 C. 슬레이터가 처음 제안
- 이후 여러 과학자들에 의해 개선되고 확장됨

## 관련 개념

- 유효 핵전하
- 차폐 효과
- 원자 궤도함수

## 참고문헌

1. Slater, J. C. (1930). Atomic Shielding Constants. Physical Review, 36(1), 57-64.
2. Levine, I. N. (2008). Quantum Chemistry. Pearson Prentice Hall.