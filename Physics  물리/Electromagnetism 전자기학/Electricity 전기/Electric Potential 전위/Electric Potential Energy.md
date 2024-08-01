---
aliases:
  - 전기 퍼텐셜 에너지
category:
  - 물리학
  - 전자기학
related_concepts:
  - 전기장
  - 전위차
  - 정전기 에너지
tags:
  - 전자기학
  - 전기
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
# 전기 퍼텐셜 에너지
## 정의
퍼텐셜 에너지란 역장(force field) 속의 어떤 물체가 특정 위치에서 갖는 스칼라 값을 의미한다. 
전기 퍼텐셜 에너지는 


## 수학적 설명
*퍼텐셜 에너지에 대한 자세한 내용은 [[Potential Energy|문서]] 참고*

퍼텐셜 에너지란 보존력에 대한 선적분의 값이다. 
$$U(r)=-\int_{r_{0}}^{r}\vec{F}\cdot d\vec{r}$$
보존력은 경로에 무관므로 시작과 끝의 상태만 알면 된다. 그러므로 최단 거리 경로를 통한 [[line integral|선적분이]] 간편할 것이다.
이때, 힘을 쿨롱 힘으로 가정하고 계산해보도록 하자. 
$$
\begin{align}
U(r)&=-\int_{r_{0}}^{r}\frac{1}{4\pi\varepsilon_{0}}\frac{Q\cdot q}{r^{2}}\cdot d\vec{r}
\\&=-\frac{Q\cdot q}{4\pi\varepsilon_{0}}[-\frac{1}{r}]_{r_{0}}^{r}
\\&=\frac{Q\cdot q}{4\pi\varepsilon_{0}}(\frac{1}{r}-\frac{1}{r_{0}})
\end{align}
$$
![[electric_potential_2d.gif|400]]
위의 식에서는 전하를 지닌 입자 $q$를 입자를 전기장의 영향 내의 $r_{0}$에서 $r$로 이동시키는 것인데,
일반적인 가정의 경우 먼 곳에서 위치 $r$로 가져다 놓는 것으로 가정하므로 $r_{0}=\infty$로 바꿔 생각해보면 다음과 같이 간소화 할 수 있다.
$$U_{elec.}(r)=\frac{Q\cdot q}{4\pi\varepsilon_{0}r}$$
