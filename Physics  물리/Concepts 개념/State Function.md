---
aliases:
  - 열역학적 상태함수
category:
  - 열역학
related_concepts:
  - 경로함수
  - 엔탈피
  - 엔트로피
  - 깁스 자유 에너지
tags:
  - 열역학
  - 화학
  - 물리화학
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
# 상태함수

## 정의

상태함수는 시스템의 현재 상태에만 의존하고, 그 상태에 도달하는 경로와는 무관한 열역학적 성질이다. 

## 주요 특징

- 경로 독립적: 초기 상태에서 최종 상태로 가는 과정과 무관하다.
- 정확한 값 측정 가능: 시스템의 현재 상태만 알면 정확히 계산할 수 있다.
- 순환 과정에서의 변화량은 0이다.

## 예시

대표적인 상태함수들:

- 내부 에너지 (U)
- [[Enthalpy|엔탈피 (H) ]]
- [[Entropy|엔트로피 (S)]]
- 깁스 자유 에너지 (G)

## 수학적 표현

상태함수 X의 미분은 완전 미분이 된다:

$$ dX = \left(\frac{\partial X}{\partial V}\right)_T dV + \left(\frac{\partial X}{\partial T}\right)_V dT $$

## 상태함수 vs 경로함수  

상태함수와 대비되는 개념으로 경로함수가 있다:

| 상태함수 | 경로함수 |
|----------|----------|
| 경로 독립적 | 경로 의존적 |
| 순환과정 변화량 = 0 | 순환과정 변화량 ≠ 0 |
| 정확한 값 측정 가능 | 변화량만 측정 가능 |

## 상태함수의 중요성

1. 열역학 제1법칙 표현: ΔU = q + w

2. 열역학적 포텐셜 정의:
   - 엔탈피 기준$$H = U + PV$$
   - 자유에너지 (엔트로피와 엔탈피)$$G = H - TS$$

3. 자발성[^1] 판단 기준 제공:
   - ΔG < 0 이면 자발적 반응

4. 화학 평형 이해:
   - ΔG = 0 일 때 평형 상태

## 다이어그램



상태함수 X는 경로와 무관하게 초기상태와 최종상태만으로 결정되지만, 경로함수 Y는 거치는 경로에 따라 값이 달라진다.

상태함수의 개념을 이해하면 열역학 시스템의 변화를 쉽게 분석하고 예측할 수 있다. 이는 화학 반응의 자발성, 평형, 에너지 변화 등을 이해하는 데 핵심이 된다.


[^1]: Spontaneity