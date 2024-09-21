---
aliases:
  - 분석 감도
  - 검출 감도
category:
  - 분석화학
related_concepts:
  - 검출한계
  - 정량한계
  - 선형성
  - 신호
tags:
  - 분석화학
  - 기기분석
  - 데이터
  - 화학
---

```table-of-contents
title: 
style: nestedList # TOC style (nestedList|nestedOrderedList|inlineFirstLevel)
minLevel: 0 # Include headings from the specified level
maxLevel: 0 # Include headings up to the specified level
includeLinks: true # Make headings clickable
debugInConsole: false # Print debug info in Obsidian console
```

# 감도 (Sensitivity)

## 정의
분석화학에서의 감도란 분석 대상의 농도 변화에 대한 측정 신호의 변화 정도를 의미한다.
이는 즉 신호와 농도의 검정곡선의 기울기로 표현. 이러한 정의를 적용하면 높은 감도는 작은 농도 변화도 감지 가능함을 의미한다.

## 상세 설명
감도는 분석 방법이나 기기의 성능을 나타내는 중요한 지표다. 높은 감도는 낮은 농도의 분석물질도 정확하게 측정할 수 있음을 의미한다. 감도는 신호와 밀접한 관련이 있으며, 일반적으로 신호 대 농도의 비율로 표현된다.
다만 기기 혹은 분석 방법에서 감지 혹은 검출 가능한 분석 대상의 최소한의 양 혹은 농도를 의미하는 검출 한계 (Detection limit; Limit of Detection; LOD)와 헷갈리지 않도록 유의하자. 

### 감도와 신호의 관계
신호(S)는 일반적으로 분석물질의 농도 $[A]$ 에 비례한다.

$$ S = k_{A}[A] + b $$

여기서 $k_{A}$는 감도, $b$는 $y$ 절편이다. 따라서 감도는 다음과 같이 정의된다:

$$ k_{A} = \frac{\Delta S}{\Delta [A]}=\text{Sensitivity} $$

### 계산 방법
여러 농도의 표준 용액을 측정하여 신호($S$) vs 농도($C$ 혹은 $[A]$) 검정 곡선(Calibration graph; Calibraiton curve)를 작성한다. 
이후 선형 회귀 분석을 통해 그래프의 기울기를 계산하면 신호의 감도를 구할 수 있다. 

#### 예시
[[Chromatography|크로마토그래피]]에서 피크 면적(A)과 농도(C) 관계:

| 농도 (ppm) | 피크 면적 |
|------------|-----------|
| 1          | 100       |
| 2          | 205       |
| 3          | 300       |
| 4          | 410       |
| 5          | 500       |

선형 회귀 분석 결과: A = 100C + 5

이 경우 감도는 100 area units/ppm이다.

### 영향을 미치는 요인
1. 기기의 성능
2. 분석 방법
3. 매트릭스 효과
4. 신호 대 잡음비

## 관련 개념
- [[Limit of Detection|검출 한계]]
- [[정량한계]]
- [[선형성]]
- [[Signal|신호]]

## 여담

감도는 분석 방법의 성능을 평가하는 중요한 지표지만, 단독으로 사용되면 안 된다. 검출한계, 정밀도, 정확도 등 다른 성능 지표들과 함께 고려해야 한다.

## 참고문헌
1. Harris, D.C. (2015). Quantitative Chemical Analysis. W.H. Freeman and Company.
2. Skoog, D.A., West, D.M., Holler, F.J., Crouch, S.R. (2013). Fundamentals of Analytical Chemistry. Cengage Learning.

