---
aliases:
  - 오차 전파
  - 불확실성 전파
  - 불확도 전파
category:
  - 오차 분석
  - 통계
  - 분석화학
related_concepts:
  - 표준편차
  - 분산
  - 공분산
tags:
  - 통계학
  - 분석화학
  - 데이터
  - 수학
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

# 불확도 전파 (Propagation of Uncertainty)

## 정요

오차 전파는 측정된 변수들의 불확실성이 어떻게 최종 계산 결과의 불확실성에 영향을 미치는지 계산하는 방법이다. 여러 변수를 포함하는 함수에서 각 변수의 오차가 최종 결과의 오차에 어떻게 기여하는지 분석할 수 있다.

## 핵심 원리

1. 각 변수의 불확실성은 독립적이며 무작위적이라고 가정한다.
2. 오차는 일반적으로 표준편차로 표현한다.
3. 변수들 간의 상관관계가 없다고 가정한다(공분산 = 0).
4. 테일러 급수 전개의 1차항까지만 고려한다.

## 수학적 표현

함수 $f(x,y,...)$에 대해 변수 $x,y,...$의 불확실성을 $\delta x, \delta y, ...$라고 할 때, $f$의 불확실성 $\delta f$는 다음과 같이 계산한다:

$$\delta f = \sqrt{\left(\frac{\partial f}{\partial x}\delta x\right)^2 + \left(\frac{\partial f}{\partial y}\delta y\right)^2 + ...}$$

### 여러 종류의 연산에서

#### 덧셈/뺄셈

$f = x \pm y$인 경우:

$$\delta f = \sqrt{(\delta x)^2 + (\delta y)^2}$$

예: $x = 10 \pm 0.1$, $y = 5 \pm 0.2$일 때 $f = x + y$의 불확실성
$$\delta f = \sqrt{0.1^2 + 0.2^2} = 0.22$$

#### 곱셈/나눗셈 

$f = xy$ 또는 $f = x/y$인 경우:

$$\frac{\delta f}{|f|} = \sqrt{\left(\frac{\delta x}{x}\right)^2 + \left(\frac{\delta y}{y}\right)^2}$$

예: $x = 10 \pm 0.1$, $y = 5 \pm 0.2$일 때 $f = xy$의 상대 불확실성
$$\frac{\delta f}{f} = \sqrt{\left(\frac{0.1}{10}\right)^2 + \left(\frac{0.2}{5}\right)^2} = 0.0412$$
$$\delta f = 0.0412 \times (10 \times 5) = 2.06$$

#### 거듭제곱

$f = x^n$인 경우:

$$\frac{\delta f}{|f|} = |n| \frac{\delta x}{|x|}$$

예: $x = 10 \pm 0.1$일 때 $f = x^2$의 불확실성
$$\frac{\delta f}{f} = 2 \times \frac{0.1}{10} = 0.02$$
$$\delta f = 0.02 \times 10^2 = 2$$

#### 로그함수

$f = \ln(x)$인 경우:

$$\delta f = \frac{\delta x}{|x|}$$

예: $x = 100 \pm 1$일 때 $f = \ln(x)$의 불확실성
$$\delta f = \frac{1}{100} = 0.01$$

#### 지수함수

$f = e^x$인 경우:

$$\delta f = |f| \delta x = e^x \delta x$$

예: $x = 2 \pm 0.1$일 때 $f = e^x$의 불확실성
$$\delta f = e^2 \times 0.1 \approx 0.738$$

#### 삼각함수

$f = \sin(x)$인 경우:

$$\delta f = |\cos(x)| \delta x$$

예: $x = \pi/4 \pm 0.01$일 때 $f = \sin(x)$의 불확실성
$$\delta f = |\cos(\pi/4)| \times 0.01 \approx 0.00707$$

#### 복합함수

$f = \sqrt{x^2 + y^2}$인 경우:

$$\delta f = \sqrt{\left(\frac{x\delta x}{\sqrt{x^2 + y^2}}\right)^2 + \left(\frac{y\delta y}{\sqrt{x^2 + y^2}}\right)^2}$$

예: $x = 3 \pm 0.1$, $y = 4 \pm 0.1$일 때 $f = \sqrt{x^2 + y^2}$의 불확실성
$$\delta f = \sqrt{\left(\frac{3 \times 0.1}{5}\right)^2 + \left(\frac{4 \times 0.1}{5}\right)^2} \approx 0.07$$


## 증명

테일러 급수 전개를 이용하여 증명할 수 있다. $f(x,y)$의 전개식:

$$f(x+\delta x, y+\delta y) = f(x,y) + \frac{\partial f}{\partial x}\delta x + \frac{\partial f}{\partial y}\delta y + \text{(고차항)}$$

고차항을 무시하고 양변에서 $f(x,y)$를 빼면:

$$\delta f = \frac{\partial f}{\partial x}\delta x + \frac{\partial f}{\partial y}\delta y$$

이 식의 양변을 제곱하고 기댓값을 취하면 최종 공식을 얻을 수 있다.

## 주의사항

1. 변수들이 독립적이지 않은 경우 공분산 항을 포함해야 한다.
2. 비선형성이 큰 함수의 경우 고차항을 고려해야 할 수 있다.
3. 불확실성이 큰 경우 몬테카를로 시뮬레이션 등 다른 방법을 고려해야 한다.
4. 로그, 지수, 삼각함수 등 비선형 함수의 경우 함수의 특성을 고려해야 한다.

## 관련 개념

- [[Standard Deviation|표준편차]]
- [[분산]]
- [[공분산]]
- [[테일러 급수]]

## 참고문헌

1. Taylor, J. R. (1997). An Introduction to Error Analysis. University Science Books.
2. Bevington, P. R., & Robinson, D. K. (2003). Data Reduction and Error Analysis for the Physical Sciences. McGraw-Hill.
3. Ku, H. H. (1966). Notes on the use of propagation of error formulas. Journal of Research of the National Bureau of Standards, 70C(4), 263-273.



## 증명

테일러 급수 전개를 이용하여 증명할 수 있다. $f(x,y)$의 전개식:

$$f(x+\delta x, y+\delta y) = f(x,y) + \frac{\partial f}{\partial x}\delta x + \frac{\partial f}{\partial y}\delta y + \text{(고차항)}$$

고차항을 무시하고 양변에서 $f(x,y)$를 빼면:

$$\delta f = \frac{\partial f}{\partial x}\delta x + \frac{\partial f}{\partial y}\delta y$$

이 식의 양변을 제곱하고 기댓값을 취하면 최종 공식을 얻을 수 있다.

## 주의사항


