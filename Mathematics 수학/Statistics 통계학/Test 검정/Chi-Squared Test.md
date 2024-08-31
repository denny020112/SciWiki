---
aliases:
  - χ² 검정
  - chi-square test
category:
  - 통계학
  - 가설검정
related_concepts:
  - 독립성 검정
  - 적합도 검정
  - 분할표 분석
  - 데이터 과학
  - 가설검정
tags:
  - 검정
  - 데이터
  - 수학
  - 통계학
---

```table-of-contents
title: 
style: nestedList # TOC style (nestedList|nestedOrderedList|inlineFirstLevel)
minLevel: 0 # Include headings from the specified level
maxLevel: 0 # Include headings up to the specified level
includeLinks: true # Make headings clickable
debugInConsole: false # Print debug info in Obsidian console
```
# 카이-제곱 검정

## 정의 및 개요
카이제곱 검정은 1900년 칼 피어슨에 의해 개발되었다. 카이제곱 검정은 범주형 데이터의 분석에 사용되는 통계적 가설검정 방법이다. 관찰된 빈도와 기대 빈도 사이의 차이를 바탕으로 귀무가설을 검정한다.

## 핵심 원리
1. 관찰 빈도와 기대 빈도의 차이 계산
2. 카이제곱 통계량 계산
3. 자유도에 따른 임계값과 비교
4. 유의확률(p-value) 계산 및 해석

## 상세 설명
카이제곱 검정은 주로 세 가지 목적으로 사용된다:

1. 적합도 검정: 관찰된 빈도가 기대되는 이론적 분포와 일치하는지 검정
2. 독립성 검정: 두 범주형 변수 사이의 관련성 유무를 검정
3. 동질성 검정: 여러 집단의 분포가 동일한지 검정

검정 통계량은 다음 공식으로 계산한다:

$$\chi^2 = \sum_{i=1}^n \frac{(O_i - E_i)^2}{E_i}$$

여기서 $O_i$는 관찰 빈도, $E_i$는 기대 빈도를 나타낸다.

## 수학적 표현
카이제곱 분포의 확률밀도함수:

$$f(x) = \frac{1}{2^{k/2}\Gamma(k/2)} x^{k/2-1}e^{-x/2}$$

여기서 $k$는 자유도, $\Gamma$는 감마 함수를 나타낸다.

## 적용 예시
- 주사위의 공정성 검정
- 성별과 직업 선택의 독립성 검정
- 여러 지역의 정치적 성향 분포 비교
- 마케팅: 고객 선호도 분석
- 의학: 질병과 위험 요인의 관련성 연구
- 품질 관리: 제품 불량률 분석

## 한계와 예외
- 기대 빈도가 5 미만인 셀이 전체의 20%를 넘으면 검정력이 떨어진다.
- 표본 크기가 매우 크면 실질적으로 의미 없는 차이도 통계적으로 유의하게 나올 수 있다.
- 연속형 변수에는 직접 적용할 수 없다.

## 여담
- 카이제곱 검정은 간단하면서도 강력한 통계적 도구이지만, 결과 해석 시 항상 실제적 의미를 고려해야 한다. 또한 표본 크기와 기대 빈도의 조건을 항상 확인해야 한다.

## 관련 개념
- [[피셔의 정확 검정]]
- [[맥니마 검정]]
- [[코크란-아미티지 검정]]

## 참고문헌
1. Pearson, K. (1900). On the criterion that a given system of deviations from the probable in the case of a correlated system of variables is such that it can be reasonably supposed to have arisen from random sampling. The London, Edinburgh, and Dublin Philosophical Magazine and Journal of Science, 50(302), 157-175.
2. Agresti, A. (2018). An introduction to categorical data analysis. John Wiley & Sons.
