---
aliases:
  - 유의확률
  - 유의수준
category:
  - 통계학
  - 가설검정
related_concepts:
  - 귀무가설
  - 대립가설
  - 유의수준
  - 검정통계량
  - 통계적 추론
  - 가설검정
  - 의사결정
tags:
  - 통계학
  - 수학
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
# p-value (유의확률)

## 정의 및 개요
p-value의 개념은 1920년대 로널드 피셔에 의해 도입되었다[^1]. p-value는 귀무가설이 참일 때, 관찰된 결과나 그보다 더 극단적인 결과가 나올 확률이다. 가설검정에서 귀무가설을 기각할지 결정하는 기준으로 사용된다.

## 핵심 원리
1. 귀무가설 하에서의 확률 분포 가정
2. 관찰된 데이터의 검정통계량 계산
3. 검정통계량과 같거나 더 극단적인 값의 확률 계산
4. 계산된 확률을 p-value로 해석

## 상세 설명
p-value는 다음과 같이 해석할 수 있다:

- 작은 p-value (일반적으로 < 0.05): 귀무가설과 관찰된 데이터가 일치하지 않음을 나타낸다.
- 큰 p-value: 귀무가설과 관찰된 데이터가 일치할 가능성이 있음을 나타낸다.

p-value를 사용한 의사결정 과정:
1. 유의수준 α 설정 (보통 0.05 또는 0.01)
2. p-value 계산
3. p-value가 α보다 작으면 귀무가설 기각, 그렇지 않으면 기각하지 않음

## 수학적 표현
양측검정에서의 p-value:

$$p\text{-value} = P(|T| \geq |t| | H_0 \text{ is true})$$

여기서 $T$는 검정통계량, $t$는 관찰된 검정통계량 값, $H_0$는 귀무가설이다.



## 실험적 증거
p-value의 유용성은 다양한 실험 연구를 통해 입증되었다. 특히 의학, 심리학, 사회과학 분야에서 연구 결과의 통계적 유의성을 판단하는 주요 도구로 사용되고 있다.

## 한계와 예외
- p-value는 효과의 크기를 나타내지 않는다.
- 표본 크기가 매우 큰 경우, 실질적으로 의미 없는 차이도 통계적으로 유의하게 나올 수 있다.
- p-value를 과도하게 의존하면 제1종 오류의 위험이 있다.
- 다중검정 시 p-value의 해석에 주의가 필요하다.


## 여담
p-value는 통계적 의사결정의 중요한 도구이지만, 그 자체로 결정적인 증거가 되지는 않는다. 효과 크기, 신뢰구간, 실제적 의미 등을 함께 고려하여 종합적인 판단을 내리는 것이 중요하다. 또한 p-value를 연구의 질이나 중요성의 지표로 사용하는 것은 적절하지 않다.

## 관련 개념
- [[유의수준]]
- [[검정력]]
- [[효과 크기]]
- [[신뢰구간]]


## 참고문헌
1. Fisher, R.A. (1925). Statistical Methods for Research Workers. Oliver and Boyd.
2. Wasserstein, R.L., & Lazar, N.A. (2016). The ASA Statement on p-Values: Context, Process, and Purpose. The American Statistician, 70(2), 129-133.



[^1]: "Statistical Methods for Research Workers" (1925)