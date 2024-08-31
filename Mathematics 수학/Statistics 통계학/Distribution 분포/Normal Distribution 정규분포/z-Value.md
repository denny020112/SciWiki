---
aliases:
  - z-score
  - 표준화 점수
category:
  - 통계
  - 확률분포
related_concepts:
  - 정규분포
  - 표준정규분포
  - t-값
  - 표준편차
tags:
  - 통계학
  - 수학
  - 검정
  - 분석화학
  - 통계역학
---

```table-of-contents
title: 
style: nestedList # TOC style (nestedList|nestedOrderedList|inlineFirstLevel)
minLevel: 0 # Include headings from the specified level
maxLevel: 0 # Include headings up to the specified level
includeLinks: true # Make headings clickable
debugInConsole: false # Print debug info in Obsidian console
```

# z 값

## 정의
z 값(z-score)은 관측값이 평균으로부터 표준편차의 몇 배만큼 떨어져 있는지를 나타내는 표준화된 측정치다. 표준정규분포를 기준으로 하는 통계량이다.

## 수식
z 값의 수식은 다음과 같다:

$$ z = \frac{X - \mu}{\sigma} $$

여기서:
- $X$: 관측값
- $\mu$: 모집단 평균
- $\sigma$: 모집단 표준편차

## 특징
1. z 값의 평균은 0, 표준편차는 1이다.
2. z 값은 서로 다른 척도의 분포를 비교할 수 있게 해준다.
3. z 값의 절댓값이 클수록 평균에서 멀리 떨어진 값이다.
4. 약 68%의 데이터가 z 값 -1과 1 사이에 있다.

## 용도
1. 이상치(outlier) 탐지
2. 확률 계산
3. 서로 다른 분포의 비교
4. 표준화된 점수 산출 (예: 시험 점수의 표준화)

## t 값과의 관계
z 값은 모집단의 표준편차를 알고 있거나 표본의 크기가 충분히 클 때(일반적으로 30 이상) 사용한다. 반면 t 값은 모집단의 표준편차를 모르고 표본의 크기가 작을 때 사용한다. 표본의 크기가 커질수록 t 분포는 z 분포(표준정규분포)에 가까워진다.

## 주의사항
1. z 값 계산 시 모집단의 평균과 표준편차를 사용해야 한다. 표본 통계량을 사용할 경우 결과가 부정확할 수 있다.
2. 극단적인 z 값(예: |z| > 3)은 이상치일 가능성이 높지만, 데이터의 특성과 맥락을 고려해야 한다.
3. 정규분포를 따르지 않는 데이터에 z 값을 적용할 때는 주의가 필요하다.