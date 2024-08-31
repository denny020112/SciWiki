---
aliases:
  - Student's t-distribution
  - t-statistic
category:
  - 통계
  - 확률분포
related_concepts:
  - 정규분포
  - 표준정규분포
  - 자유도
  - z-score
tags:
  - 수학
  - 통계학
  - 분석화학
  - 통계역학
  - 데이터
---

```table-of-contents
title: 
style: nestedList # TOC style (nestedList|nestedOrderedList|inlineFirstLevel)
minLevel: 0 # Include headings from the specified level
maxLevel: 0 # Include headings up to the specified level
includeLinks: true # Make headings clickable
debugInConsole: false # Print debug info in Obsidian console
```

# t 값

## 정의
t 값은 표본의 평균과 모집단의 평균 간의 차이를 표본의 표준오차로 나눈 값이다. 표본의 크기가 작을 때(일반적으로 30 미만) 정규분포 대신 사용되는 t 분포의 기준이 되는 통계량이다.

## 수식
t 값의 수식은 다음과 같다:

$$ t = \frac{\bar{X} - \mu}{s / \sqrt{n}} $$

여기서:
- $\bar{X}$: 표본 평균
- $\mu$: 모집단 평균
- $s$: 표본 표준편차
- $n$: 표본 크기

## 특징
1. 자유도에 따라 분포의 형태가 달라진다.
2. 표본 크기가 커질수록 정규분포에 가까워진다.
3. t 분포는 정규분포보다 꼬리가 두껍다.
4. 표본 크기가 30 이상일 때는 일반적으로 z 분포로 근사할 수 있다.

## 용도
1. 소표본에서의 평균 추정
2. 두 집단 간 평균 차이 검정 (독립표본 t 검정, 대응표본 t 검정)
3. 회귀분석에서 계수의 유의성 검정

## z 값과의 관계
t 값은 표본 크기가 작을 때 z 값을 대체하여 사용한다. 표본 크기가 커질수록 t 분포는 표준정규분포(z 분포)에 수렴한다. 즉, 자유도가 무한대일 때 t 분포는 표준정규분포와 동일해진다.

## 주의사항
1. t 검정은 데이터가 정규분포를 따른다고 가정한다.
2. 표본 크기가 매우 작을 경우(n < 5) t 검정의 신뢰성이 떨어질 수 있다.
3. 큰 표본에서는 t 검정 대신 z 검정을 사용하는 것이 더 적절할 수 있다.