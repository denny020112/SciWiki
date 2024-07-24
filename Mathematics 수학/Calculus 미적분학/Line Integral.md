---
aliases:
  - 경로 적분
  - 선적분
category:
  - 미적분학
  - 벡터 해석
related_concepts:
  - 그린 정리
  - 스토크스 정리
  - 보존장
tags:
  - 적분
  - 벡터장
  - 경로
  - 수학
  - 미적분학
  - 물리
---

```table-of-contents
title: 
style: nestedList # TOC style (nestedList|nestedOrderedList|inlineFirstLevel)
minLevel: 0 # Include headings from the specified level
maxLevel: 0 # Include headings up to the specified level
includeLinks: true # Make headings clickable
debugInConsole: false # Print debug info in Obsidian console
```
# 선적분 (line integral)

## 정의
선적분은 곡선에 있는 모든 점에 대해 함수나 벡터장의 적분을 구하는 것이다. 
장(field)에 대한 선적분은 스칼라장이나 벡터장을 특정 경로 곡선 $C$를 따라 적분하는 것을 의미한다.
### 수학적 의미
변수 $s$에 대한 곡선 $C$에서의 함수 $f(x,y)$의 선적분은 다음과 같이 구분구적법[^1]으로 나타낼 수 있다. 
$$\int_{C}f(x,y)ds=\lim\limits_{|P|\to0}\sum_{i=1}^{n}f(\bar{x}_{i},\bar{y}_{i})\Delta s_{i}$$

즉, $C$라는 곡선 경로 위에서, 잘게 쪼갠 $s$에 대해 주어진 함수를 적분하면 공간상에서 우변의 값에 대응하는 면적이 나온다. 
#### 대상 확인
선적분을 할 때 중요한 것은 선적분의 대상, 즉 피함수의 성질을 판별하는 것이다.    
성질은 크게 두 가지로 나뉘는데, 피함수가 스칼라 함수인 경우와 피함수가 벡터 함수인 경우이다. 각각의 경우에는 스칼라장에서의 선적분과 벡터장에서의 선적분으로 갈리기 때문에 다르게 보아야 한다.
##### 스칼라장에서의 선적분 
![[scalar field line integral 2D.png|450]]
![[scalar field line integral 3D.png|450]]
스칼라 함수 $f(x,y)$의 선적분은 다음과 같이 정의된다:

$$ \int_C f(x,y) ds = \int_a^b f(x(t),y(t)) \sqrt{\left(\frac{dx}{dt}\right)^2 + \left(\frac{dy}{dt}\right)^2} dt $$

여기서 $(x(t),y(t))$는 곡선 $C$의 매개변수 표현이며, $a \leq t \leq b$이다.
변수 $s$에 대한 $ds$의 적분으로는 $f(x,y)$를 적절하게 계산하기에는 힘들다. 
이를 해결하기 위해  $x$ 와 $y$를 통한 [[Integration by Substitution|치환적분]]으로  계산을 할 수 있다. 
이때 곡선 경로 $C$를 잘게 쪼갠 $ds$를 다음과 같이 변환하여 계산한다.
$$ds=\sqrt{\left(\frac{dx}{dt}\right)^2 + \left(\frac{dy}{dt}\right)^2}dt$$
간단하게 종합해보면, 스칼라 함수에 대한 선적분은 다음과 같이 표현할 수 있다.
$$\int_{C}f\ ds=\int_{C}f(r(t))|r'(t)|dt$$

##### 벡터장에서의 선적분
![[vector field line integral.png|500]]
벡터장 $\mathbf{F}(x,y) = P(x,y)\mathbf{\hat{i}} + Q(x,y)\mathbf{\hat{j}}$의 선적분은 다음과 같이 정의된다:

$$ \int_C \mathbf{F} \cdot d\mathbf{r} = \int_a^b [P(x(t),y(t))\frac{dx}{dt} + Q(x(t),y(t))\frac{dy}{dt}] dt $$
즉, 벡터함수와 적분요소($dr$)의 내적이다. 
벡터장에서의 선적분이 가장 자주 활용되는 경우는 물리에서 일의 계산이다.    
아래의 예시에서 알아보자.
###### 물리적 예시: 일의 계산
*일에 대한 자세한 내용은 [[work|문서]] 참고*

일의 정의는 $$\vec{W}=\vec{F}\cdot s$$
적분형태는
$$\vec{W}=\int \vec{F}\cdot d\vec{s}$$
이를 구분구적법으로 해석하면
$$
\begin{align}
\vec{W}=\int \vec{F}\cdot d\vec{s}&=\lim\limits_{|\Delta \vec{s}|\to0}\sum_{i=1}^{n}\vec{F}_{i}\cdot\Delta \vec{s}_{i}
\\&=\int_{C}\vec{F}\cdot d\vec{s}
&&
\end{align}
$$

즉, 

## 적용 예시
- 물리학: 일의 계산. 
	- 물리 실험에서 일이나 전위차를 측정하여 선적분의 결과를 검증할 수 있다.
- 전자기학: 전위차 계산
- 유체역학: 유량 계산
## 관련 개념
- [[그린 정리]]: 폐곡선에서의 선적분은 그린 정리를 통해 영역 적분으로 변환할 수 있다.
- [[스토크스 정리]]
- [[보존장]]


## 참고문헌
1. Stewart, J. (2015). Calculus: Early Transcendentals. Cengage Learning.
2. Kreyszig, E. (2011). Advanced Engineering Mathematics. John Wiley & Sons.

[^1]: 더 엄밀히 말하자면면 리만 합으로 나타낸 것이다.