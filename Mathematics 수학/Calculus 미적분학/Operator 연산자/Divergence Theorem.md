---
aliases:
  - 발산정리
  - 가우스정리
  - Gauss's Theorem
category:
  - 벡터 미적분학
related_concepts:
  - 발산
  - 나블라
tags:
  - 수학
  - 벡터
  - 해석
  - 물리
  - 미적분학
  - 선형대수학
---

```table-of-contents
title: 
style: nestedList # TOC style (nestedList|nestedOrderedList|inlineFirstLevel)
minLevel: 0 # Include headings from the specified level
maxLevel: 0 # Include headings up to the specified level
includeLinks: true # Make headings clickable
debugInConsole: false # Print debug info in Obsidian console
```
# 발산 정리 (Divergence Theorem)

![[gauss theorem.png|450]]
## 개요 및 정의
>어떤 벡터장이 퍼져나가는 정도, 즉, 발산은 그 벡터장의 양, 선속(Flux)와 같다. 

발산정리 (divergence theorem) 혹은 가우스 정리(Gauss' theorem)라고 불린다.
벡터장의 발산과 그 벡터장의 선속을 연관짓는 정리이다. 직관적으로 말해 벡터장에서 뻗어나온 선의 수는 곧 그 주변 폐곡선 혹은 폐곡면을 뚫고 나오는 선의 수와 같다고 생각할 수 있다.

## 발산 (divergence)
### 발산의 개념
발산은 말 그대로 퍼져 나가는 정도를 말하는 것이다. 

어느 한 벡터장을 가정했을 때, 그 벡터장의 임의의 한 점에서 과연 어느 정도로 벡터가 퍼져나가는지[^1]를 알 수 있으면, 그 지점에서의 발산을 알 수 있을 것이다.

먼저 간단하게 생각해보기 위해 아래의 평면을 참고해서 생각해보도록 하자.
![[vector field divergence.png|400]]
초록색 구간으로 표현된 매우 작은, 미소(infinitesimal)[^3] 면적이 있다. 
이 미소면적에 들어오고 나가는 벡터의 양, 즉 유량(flow rate)[^2]을 고려하면 이 미소영역에서의 발산의 정도를 알 수 있을 것이다. 

그럼 이제 벡터장을 가정하는 식을 일반적으로 다음과 같이 가정하자. $$f(x,y)=P(x,y)\hat{i}+Q(x,y)\hat{j}$$
$P$와 $Q$는 각각 $x$ 그리고 $y$ 성분이다. 이때, 미소 영역의 발산량은 각각 $x$ 성분의 발산량과 $y$성분의 발산량으로 정리할 수 있을 것이다.
각 성분의 발산량은 미소영역의 각 변($\Delta x$,$\Delta y$)당 퍼져나가는 벡터의 양과 들어오는 양의 차를 통해 구할 수 있을 것이다.
$$
\begin{align}
x\text{ component divergence}\approx \frac{P(x+\Delta x, y) - P(x, y)}{\Delta x}
\\ y\text{ component divergence}\approx \frac{Q(x, y+\Delta y) - Q(x, y)}{\Delta y}
&&
\end{align}
$$

두 성분의 발산을 종합하여 이 미소영역의 발산을 구할 수 있다.
$$Divergence\approx \frac{P(x+\Delta x, y) - P(x, y)}{\Delta x} + \frac{Q(x, y+\Delta y) - Q(x, y)}{\Delta y}$$


### 2차원 발산
*관련 내용은 [[Del|나블라]] 문서의 [[Del#발산(Divergence)|발산]] 문단 참고*
위에서는 대략적으로 벡터장의 발산을 알아볼 수 있는 수학적 방법에 대하여 설명했다.
더 정밀한 계산을 위해서는 미소영역의 면적이 무한소에 가까워져야 한다.

이는 $\Delta x$와 $\Delta  y$가 0에 접근해야 한다는 것이며, 이를 식에 적용하여 나타내면: $$
\begin{align}
\lim_{\Delta x \to 0} \frac{P(x+\Delta x, y) - P(x, y)}{\Delta x} = \frac{\partial P}{\partial x}\\
\lim_{\Delta y\to 0} \frac{Q(x, y+\Delta y) - Q(x, y)}{\Delta y} = \frac{\partial Q}{\partial y}
&&
\end{align}
$$
즉, 벡터장의 각 성분에 해당하는 부분에 대한 편미분을 하는 것과 동일한 표현이 된다.
이때 각 식에 대한 편미분을 연산자로써 따로 분리한 형태로 표현을 하자면,
$$
\begin{align}
\frac{\partial }{\partial \ var.}\cdot f=\frac{\partial P}{\partial x}+\frac{\partial Q}{\partial y}
&&
\end{align}
$$
각 변수에 대해 벡터장의 각 성분을 편미분한 후 더한 것과 같다.
즉, [[del|편미분 연산자]]와 벡터장 $f$의 [[Inner Product|내적]]으로써 표현될 수 있고, 
이는 곧 나블라를 이용한 방식으로 표기를 바꿀 수 있다는 것이다.
$$\nabla\cdot f=\frac{\partial P}{\partial x}+\frac{\partial Q}{\partial y}$$

### 3차원 발산
다음과 같은 3차원에서의 벡터장을 가정했을 때
$$F(x, y, z) = F_{1}(x,y,z)\ \hat{i} + F_{2}(x,y,z)\ \hat{j} + F_{3}(x,y,z)\ \hat{k}$$
발산은 2차원에서의 경우와 동일하게 이 3차원 벡터장에 대한 나블라의 내적으로 정의할 수 있다
$$
\begin{flalign}
\nabla\cdot\mathbf{F}= \frac{\partial F_{1}}{\partial x}+\frac{\partial F_{2}}{\partial y}+\frac{\partial F_{3}}{\partial z}
&&
\end{flalign}
$$

## 발산 정리
### 2 차원 발산 정리


### 3 차원 발산 정리



[^1]: 음수의 정도로 퍼져나간다면 모여든다는 의미로 받아들여도 괜찮다
[^2]: 흐르는 양
[^3]: 그림에는 굉장히 단순한 양의 벡터들만 표현이 되었으나 실제로는 무수히 많은 벡터가 굉장히 촘촘하게 통과할 것이기 때문에 미소영역을 가정하는것이 더 정밀하다 할 수 있을 것이다.