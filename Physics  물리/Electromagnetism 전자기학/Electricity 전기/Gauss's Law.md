---
aliases:
  - Gauss's Law
  - 가우스의 정리
category:
  - 물리학
  - 전자기학
related_concepts:
  - 전기장
  - 전속
  - 전하 분포
tags:
  - 전자기학
  - 맥스웰
  - 방정식
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
# 가우스 법칙 (Gauss's Law)
![[gauss's law sphere.png|400]]
## 개요
>임의의 닫힌 표면[^1]을 통과하는 총 전기다발($\Phi E$)[^2]은 그 닫힌 표면 안의 총 전하($Q_{encl}$)를 진공 유전체($\varepsilon_{0}$)로 나눈 것과 같다

가우스 법칙은 전하와 전기장 사이의 관계를 설명하는 전자기학의 기본 법칙 중 하나이다. 이는 맥스웰 방정식의 하나로, 전하 분포와 그로 인한 전기장을 연관짓는다.

## 수학적 표현

### 적분 형태

$$ \oint_S \vec{E} \cdot d\vec{A} = \frac{Q_{enc}}{\epsilon_0} $$

여기서:
- $\vec{E}$는 전기장
- $d\vec{A}$는 닫힌 면의 미소 면적 벡터
- $Q_{enc}$는 닫힌 면 내부의 총 전하량
- $\epsilon_0$는 진공의 유전율

### 미분 형태

$$ \nabla \cdot \vec{E} = \frac{\rho}{\epsilon_0} $$

여기서 $\rho$는 전하 밀도이다.

## 원리 및 유도 (Derivation)

가우스 법칙은 [[Coulomb's Law|쿨롱의 법칙]]으로부터 유도할 수 있다. 
### 구 가우스 표면 (Spherical Gaussian surface)
밑의 경우에는 가장 간단한 구의 표면을 가우스면으로 전제하고 유도하였다. 유도 과정은 다음과 같다:

점전하에 의한 전기장 $\vec{E}$ 는 쿨롱의 법칙을 통해 구할 수 있다
 $$
		\begin{flalign} 
		\vec{E} &= \frac{\vec{F}}{q_{unit}}
		\\&=(\frac{1}{4\pi\varepsilon_0} \frac{q\cdot q_{unit}}{r^2} \hat{r})/q_{unit} 
		\\&= \frac{1}{4\pi\varepsilon_0} \frac{q}{r^2} \hat{r} 
		&&
		\end{flalign} $$

이때 반지름 $r$인 구면 가우스 표면을 가정하여 전기 선속(flux)을 계산한다.

$$
		\begin{flalign} 
		\Phi_{E} &= \oint_{S}\vec{E}\cdot d\vec{A} 
		\\&= \frac{q}{4\pi\varepsilon_0}\oint_{S} \frac{1}{r^{2}} \hat{r}\cdot d\vec{A} 
		&&
		\end{flalign} 
$$

구면의 면적 $d\vec{A}$는 항상 $\hat{r}$ 방향, 즉 전기장 $\vec{E}$의 방향과 일치하므로, 
방향에 대한 고려를 하지 않고 $dA$로 간소화가 가능하다.

$$ \begin{flalign}
\Phi_E &= \frac{q}{4\pi\epsilon_0} \oint_S \frac{1}{r^2} dA 
\\&= \frac{q}{4\pi\varepsilon_0} \frac{1}{r^2} (4\pi r^2)
\\&= \frac{q}{\varepsilon_0} 
&&
\end{flalign}
$$

### 비구면 가우스 표면 (Nonspherical Gaussian surface)

위의 구형의 폐곡면을 가정했을때의 정리를 일반화하면 [[Divergence Theorem|가우스 법칙]]의 적분 형태를 얻는다.

   $$ \oint_S \vec{E} \cdot d\vec{A} = \frac{Q_{enc}}{\varepsilon_0} $$

발산 정리를 적용하면 미분 형태를 얻을 수 있다:

   $$ \oint_S \vec{E} \cdot d\vec{A} = \int_V (\nabla \cdot \vec{E}) dV = \frac{Q_{enc}}{\varepsilon_0} = \int_V \frac{\rho}{\varepsilon_0} dV $$

   따라서, $\nabla \cdot \vec{E} = \frac{\rho}{\varepsilon_0}$
#### 시각적 설명
![[gaussian surface.png|500]]
위 그림에서도 보이듯이 중앙의 점전하를 모두 포함하는 형태의 폐곡면을 상정했을 때, 점전하에서 뻗어나오는 전기장의 선 숫자와 여러 형태의 폐곡면을 지나가는 선의 숫자 (선속)은 다르지 않다는 것을 시각적으로 이해할 수 있다.
## 적용과 응용

1. 대칭성이 높은 전하 분포의 전기장 계산
   - 구 대칭 전하 분포
   - 원통형 전하 분포
   - 무한 평면 전하 분포

2. 정전기학 문제 해결
   - 도체 내부와 표면의 전하 분포
   - 유전체 내부의 전기장

3. 맥스웰 방정식의 일부로서 전자기 이론의 기초

## 물리적 의의

1. 전하와 전기장의 관계를 설명한다. 전하가 전기장의 근원임을 명확히 한다.

2. 계산 효율성: 대칭성이 높은 문제에서 전기장 계산을 단순화한다.

3. 전자기 이론의 기초: 맥스웰 방정식의 핵심 구성 요소이다.

4. 물리적 직관 제공: 전기 선속과 전하의 관계를 시각화할 수 있다.

## 한계점

1. 비대칭 전하 분포: 대칭성이 낮은 경우 적용이 어렵다.

2. 시간 변화하는 자기장: 정자기 상태에서만 정확하다. (맥스웰-암페어 법칙에서 다룸)

3. 경계 조건: 매질의 경계에서 추가적인 고려가 필요하다.

가우스 법칙은 전자기학의 근간을 이루는 중요한 법칙으로, 전하와 전기장의 관계를 명확히 설명하며 다양한 전자기 현상을 이해하는 데 핵심적인 역할을 한다.


[^1]: 폐곡면이라고 한다. 가우스의 이름을 따서 가우스 표면 혹은 가우스면(Gaussian surface)이라고도 한다
[^2]: 전기선속