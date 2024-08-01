---
aliases:
  - t 검정
  - Student's t-test
category:
  - 통계학
  - 가설검정
related_concepts:
  - 정규분포
  - 표준오차
  - 자유도
  - 중심극한정리
  - 모수검정
  - 평균비교
  - 소표본
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
# t-test

## 정의
t-test는 두 집단의 평균을 비교하거나 한 집단의 평균을 특정 값과 비교하는 통계적 가설검정 방법이다. 소표본에서도 사용 가능하며, 정규분포를 따르는 모집단을 가정한다.

## 핵심 원리
1. 표본 평균과 표준오차 계산
2. t 통계량 계산
3. 자유도에 따른 t 분포의 임계값과 비교
4. 유의확률(p-value) 계산 및 해석

## 상세 설명
t-test는 주로 세 가지 유형으로 나뉜다:

1. 일표본 t-test: 한 집단의 평균을 특정 값과 비교
2. 독립표본 t-test: 두 독립된 집단의 평균을 비교
3. 대응표본 t-test: 동일 집단의 전후 측정값 비교

t 통계량은 다음과 같이 계산한다:

일표본 t-test의 경우: $$t = \frac{\bar{x} - \mu_0}{s / \sqrt{n}}$$

여기서 $\bar{x}$는 표본 평균, $\mu_0$는 비교하려는 값, $s$는 표본 표준편차, $n$은 표본 크기다.

## 수학적 표현
t 분포의 확률밀도함수:

$$f(t) = \frac{\Gamma(\frac{\nu+1}{2})}{\sqrt{\nu\pi}\Gamma(\frac{\nu}{2})} (1 + \frac{t^2}{\nu})^{-\frac{\nu+1}{2}}$$

여기서 $\nu$는 자유도, $\Gamma$는 감마 함수를 나타낸다.

## 역사적 배경
t-test는 1908년 윌리엄 고셋이 기네스 양조장에서 일하며 개발했다. 당시 회사 정책으로 인해 'Student'라는 필명으로 발표했으며, 이로 인해 'Student's t-test'라고도 불린다.


## 한계와 예외
- 표본 크기가 매우 작을 경우 정규성 가정이 중요해진다.
- 두 집단의 분산이 크게 다를 경우 Welch's t-test를 사용해야 한다.
- 다중 비교 시 제1종 오류가 증가할 수 있으므로 보정이 필요하다.

## 관련 개념
- [[분산분석(ANOVA)]]
- [[Mann-Whitney U test]]
- [[Wilcoxon 부호순위 검정]]

## 학습 팁
- t 분포와 정규분포의 차이점을 이해하는 것이 중요하다.
- 자유도의 개념과 그 영향을 잘 파악해야 한다.
- 실제 데이터를 사용해 각 유형의 t-test를 수행해보는 것이 도움된다.

## 연습 문제
1. 한 반 학생 25명의 키 평균이 170cm라고 주장한다. 실제 측정 결과 평균이 168cm, 표준편차가 5cm였다. 이 주장이 옳은지 검정하시오.

2. 두 집단 A와 B의 데이터가 다음과 같다:
   A: 15, 17, 20, 22, 24
   B: 14, 16, 18, 20, 22
   두 집단의 평균에 유의한 차이가 있는지 검정하시오.

## 참고문헌
1. Student. (1908). The probable error of a mean. Biometrika, 6(1), 1-25.
2. Zimmerman, D. W. (1997). A note on interpretation of the paired-samples t test. Journal of Educational and Behavioral Statistics, 22(3), 349-360.

## 여담
- t-test는 간단하면서도 강력한 통계적 도구지만, 항상 가정의 충족 여부를 확인해야 한다. 또한 효과 크기(effect size)를 함께 보고하는 것이 결과의 실질적 의미를 해석하는 데 도움이 된다.
- t-test의 유효성은 다양한 실험과 시뮬레이션 연구를 통해 입증되었다. 특히 정규성 가정이 위배되는 경우에도 상당히 강건한(robust) 결과를 보인다는 것이 알려져 있다.