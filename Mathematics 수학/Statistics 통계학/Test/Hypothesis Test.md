---
alias: [가설검정, 통계적 추론]
category: [통계학, 추론통계]
related_concepts: [유의수준, p-값, 검정력, 제1종 오류, 제2종 오류]
tags: [통계적 추론, 의사결정, 데이터 분석]
---

```table-of-contents
title: 
style: nestedList # TOC style (nestedList|nestedOrderedList|inlineFirstLevel)
minLevel: 0 # Include headings from the specified level
maxLevel: 0 # Include headings up to the specified level
includeLinks: true # Make headings clickable
debugInConsole: false # Print debug info in Obsidian console
```
# 가설 검정 (Hypothesis Test)

## 정의 및 개요
가설검정은 표본 데이터를 사용하여 모집단에 대한 가설의 타당성을 평가하는 통계적 추론 방법이다. 귀무가설과 대립가설을 설정하고, 표본 데이터를 바탕으로 귀무가설을 기각할지 여부를 결정한다.
가설검정의 기본 개념은 20세기 초 로널드 피셔에 의해 제시되었다. 가설검정의 현대적 틀은 에곤 피어슨, 예지 네이만 등에 의해 제시되었다. 

## 핵심 원리
1. 귀무가설(H₀)과 대립가설(H₁) 설정
2. 유의수준(α) 선택
3. 검정통계량 계산
4. p-값 계산 또는 기각역 설정
5. 결론 도출

## 상세 설명
가설검정의 과정은 다음과 같다:

1. 귀무가설 설정: 일반적으로 "차이가 없다" 또는 "관계가 없다"는 주장을 귀무가설로 설정한다.
2. 대립가설 설정: 연구자가 입증하고자 하는 주장을 대립가설로 설정한다.
3. 유의수준 선택: 보통 0.05 또는 0.01을 사용한다.
4. 검정통계량 계산: 표본 데이터를 바탕으로 검정통계량(예: t, z, F, χ²)을 계산한다.
5. p-값 계산: 귀무가설이 참일 때 관찰된 결과나 더 극단적인 결과가 나올 확률을 계산한다.
6. 결론 도출: p-값이 유의수준보다 작으면 귀무가설을 기각하고, 그렇지 않으면 기각하지 않는다.

## 수학적 표현
p-값의 정의:

$$p\text{-value} = P(T \geq t | H_0 \text{ is true})$$

여기서 $T$는 검정통계량, $t$는 관찰된 검정통계량 값이다.


## 한계와 예외
- 유의수준의 임의성
- 제1종 오류와 제2종 오류의 트레이드오프
- 표본 크기가 매우 큰 경우 실질적으로 무의미한 차이도 통계적으로 유의하게 나올 수 있음
- 다중검정 문제

## 관련 개념
- [[신뢰구간]]
- [[베이지안 추론]]
- [[효과 크기]]
- [[검정력 분석]]

## 여담
가설검정은 통계적 추론의 핵심 도구지만, 결과 해석 시 주의가 필요하다. p-값만으로 결론을 내리기보다는 효과 크기, 신뢰구간 등을 함께 고려해야 한다. 또한 실제적 의미와 통계적 유의성을 구분하는 것이 중요하다.

## 참고문헌
1. Fisher, R.A. (1925). Statistical Methods for Research Workers. Oliver and Boyd.
2. Neyman, J., & Pearson, E. S. (1933). On the Problem of the Most Efficient Tests of Statistical Hypotheses. Philosophical Transactions of the Royal Society A, 231(694–706), 289–337.
