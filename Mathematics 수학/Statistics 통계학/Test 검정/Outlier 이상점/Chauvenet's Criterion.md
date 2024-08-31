---
aliases:
  - Chauvenet's Criterion
  - Chauvenet's Test
  - 쇼브네 검정
category:
  - 통계학
  - 이상치 검출
related_concepts:
  - 딕슨 Q 테스트
  - 쇼브네 검정
tags:
  - 통계학
  - 수학
  - 분석화학
  - 화학
  - 이상점
---

```table-of-contents
title: 
style: nestedList # TOC style (nestedList|nestedOrderedList|inlineFirstLevel)
minLevel: 0 # Include headings from the specified level
maxLevel: 0 # Include headings up to the specified level
includeLinks: true # Make headings clickable
debugInConsole: false # Print debug info in Obsidian console
```

# 쇼브네 검정

## 정의

정규 분포를 따르는 데이터셋에서 이상치를 식별하기 위한 통계적 방법

## 핵심 원리

1. 데이터의 평균과 표준편차를 계산한다.
2. 각 데이터 포인트에 대해 표준 편차 단위로 평균으로부터의 거리를 계산한다.
3. 이 거리에 해당하는 정규 분포의 확률을 구한다.
4. 데이터 포인트 수와 확률을 곱한 값이 0.5보다 작으면 이상치로 판단한다.

## 수학적 표현

데이터 포인트 x에 대한 Chauvenet's 기준:

$$P(|x - \mu| > |x_i - \mu|) \cdot N < 0.5$$

여기서 $\mu$는 평균, N은 데이터 포인트의 수다.

## 적용 예시

데이터셋: 12, 14, 14, 15, 16, 17, 18, 32

평균 = 17.25, 표준편차 = 6.23 32에 대한 Z-점수 = (32 - 17.25) / 6.23 = 2.37

P(|Z| > 2.37) ≈ 0.0178 0.0178 * 8 = 0.1424 < 0.5

따라서 32는 Chauvenet's 기준에 따라 이상치로 판단된다.

## 장단점

장점:

- 계산이 비교적 간단하다
- 정규 분포를 따르는 데이터에 효과적이다

단점:

- 정규성 가정이 필요하다
- 작은 표본 크기에서는 신뢰성이 떨어질 수 있다
- 한 번에 하나의 이상치만 제거할 수 있다

## 관련 개념

- 딕슨 Q 테스트
- 그럽스 테스트