---
aliases:
  - confidence interval
  - CI
category:
  - 통계학
  - 추정
related_concepts:
  - 점추정
  - 표준오차
  - 유의수준
  - 표본분포
  - 구간추정
  - 불확실성
  - 모수추정
tags:
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
# 신뢰구간 (Confidence Interval)

## 정의 및 개요
신뢰구간은 1937년 예지 네이만에 의해 처음 제안된 개념이다. 신뢰구간은 모수의 참값이 일정한 확률로 포함될 것으로 기대되는 구간 추정치다. 점추정치의 불확실성을 나타내며, 구간의 폭은 추정의 정밀도를 반영한다.

## 핵심 원리
1. 표본 통계량 계산
2. 표준오차 추정
3. 신뢰수준 선택
4. 임계값 결정
5. 신뢰구간 계산

## 상세 설명
신뢰구간은 일반적으로 다음과 같은 형태를 가진다:

(점추정치) ± (임계값) × (표준오차)

예를 들어, 모평균 μ에 대한 95% 신뢰구간은:

$$\bar{x} \pm t_{\alpha/2, n-1} \cdot \frac{s}{\sqrt{n}}$$

여기서 $\bar{x}$는 표본평균, $s$는 표본표준편차, $n$은 표본크기, $t_{\alpha/2, n-1}$는 자유도 $n-1$인 t-분포의 임계값이다.

신뢰수준(예: 95%)은 동일한 방법으로 표본을 반복 추출할 때, 구간에 모수가 포함될 비율을 의미한다.

## 수학적 표현
모평균 μ에 대한 $(1-\alpha)100\%$ 신뢰구간:

$$P(\bar{x} - t_{\alpha/2, n-1} \cdot \frac{s}{\sqrt{n}} \leq \mu \leq \bar{x} + t_{\alpha/2, n-1} \cdot \frac{s}{\sqrt{n}}) = 1-\alpha$$



## 한계와 예외
- 신뢰구간의 해석에 주의가 필요하다. 95% 신뢰구간은 모수가 95% 확률로 구간 안에 있다는 의미가 아니다.
- 비정규 분포나 작은 표본 크기의 경우 정확도가 떨어질 수 있다.
- 복잡한 통계 모델에서는 신뢰구간 계산이 어려울 수 있다.



## 여담
- 신뢰구간은 점추정치만으로는 알 수 없는 추정의 정밀도와 불확실성에 대한 중요한 정보를 제공한다. 따라서 연구 결과를 보고할 때 점추정치와 함께 신뢰구간을 제시하는 것이 좋다. 또한 신뢰구간은 가설검정의 결과를 시각적으로 이해하는 데도 도움을 준다.
- 로널드 피셔의 유의성 검정에 대한 대안으로 발전되었다.


## 관련 개념
- [[표준오차]]
- [[가설검정]]
- [[베이지안 신용구간]]
- [[부트스트랩 방법]]
## 참고문헌
1. Neyman, J. (1937). Outline of a Theory of Statistical Estimation Based on the Classical Theory of Probability. Philosophical Transactions of the Royal Society A, 236(767), 333-380.
2. Cumming, G., & Finch, S. (2005). Inference by Eye: Confidence Intervals and How to Read Pictures of Data. American Psychologist, 60(2), 170-180.