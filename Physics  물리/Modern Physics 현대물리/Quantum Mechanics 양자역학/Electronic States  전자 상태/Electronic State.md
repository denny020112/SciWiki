---
aliases:
  - 전자 구조
  - 원자 오비탈
category:
  - 양자화학
  - 원자물리학
  - 화학
  - 물리학
related_concepts:
  - 파동함수
  - 슈뢰딩거 방정식
  - 양자수
  - 원자단위
  - 전자
tags:
  - 원자구조
  - 에너지준위
  - 화학
  - 물리
  - 물리화학
  - 양자역학
  - 양자화학
---

```table-of-contents
title: 
style: nestedList # TOC style (nestedList|nestedOrderedList|inlineFirstLevel)
minLevel: 0 # Include headings from the specified level
maxLevel: 0 # Include headings up to the specified level
includeLinks: true # Make headings clickable
debugInConsole: false # Print debug info in Obsidian console
```

# 전자상태 (Electronic State)

## 정의 및 개요

전자상태는 원자나 분자 내 전자의 양자역학적 상태를 말한다. 이는 파동함수로 표현되며, 슈뢰딩거 방정식의 해로 얻어진다. 전자상태는 여러 양자수로 특징지어지며, 이는 전자의 에너지, 각운동량, 스핀 등의 물리량을 결정한다.

## 수소와 수소 유사 원자의 경우

### 수소 원자의 전자상태

수소 원자는 가장 단순한 원자 시스템으로, 그 전자상태는 해석적으로 풀 수 있다. 
수소 원자의 파동함수는 다음과 같이 표현된다:

$$\psi_{nlm}(r,\theta,\phi) = R_{nl}(r)Y_{lm}(\theta,\phi)$$

여기서 $R_{nl}(r)$은 동경 함수, $Y_{lm}(\theta,\phi)$는 구면조화함수다.

#### 증명

![[hydrogen spherical plot.png|250]]

슈뢰딩거 방정식에서 시작해보도록 하자.
$$-\frac{\hbar^{2}}{2m}\nabla^{2}\psi+V(x)\psi=E\psi$$

이 때 원자핵에 의해 전자가 가지게 되는 전기 퍼텐셜 에너지는 다음과 같다. $$V(r)=-\frac{(Z\cdot e)\cdot e}{4\pi\varepsilon_{0}r}$$
슈뢰딩거 방정식에 대입하여 구면 좌표에 대하여 정리하면 
$$\underbrace{- \frac{\hbar^{2}}{2m}[\frac{1}{\sin\theta} \frac{\partial}{\partial\theta}(\sin\theta \frac{\partial}{\partial\theta})+ \frac{1}{\sin^{2}\theta} \frac{\partial^{2}}{\partial\phi^{2}}]}_{\text{angular part}}\psi+\underbrace{(-\frac{Z e^{2}}{4\pi\varepsilon_{0}r})}_{\text{radial part}}\psi=E\psi$$

해를 구할 때 변수를 분리하여 방사형 해와 각도 기반의 해를 곱하여 정리할 수 있다.
$$\psi=R(r)\times Y_{l,m_{l}}(\theta,\phi) $$

### 수소 유사한 원자의 경우

He+, Li2+ 등 수소 유사 원자 (H-like species) 원자핵과 1개의 전자로만 이루어진 구조를h 가지며, 다음과 같이 표현된다:

$$\psi_{nlm}(r,\theta,\phi) = \sqrt{\left(\frac{2Z}{na_0}\right)^3\frac{(n-l-1)!}{2n[(n+l)!]^3}}\left(\frac{2Zr}{na_0}\right)^l e^{-Zr/na_0} L_{n-l-1}^{2l+1}\left(\frac{2Zr}{na_0}\right) Y_{lm}(\theta,\phi)$$

여기서 $Z$는 원자번호, $a_0$는 보어 반지름, $L_{n-l-1}^{2l+1}$는 라게르 다항식이다.

## n=1, 2에 대한 파동함수

### 복소수 형태
1s: $$\psi_{100} = \frac{1}{\sqrt{\pi a_0^3}}e^{-r/a_0}$$

2s: $$\psi_{200} = \frac{1}{\sqrt{32\pi a_0^3}}\left(2-\frac{r}{a_0}\right)e^{-r/2a_0}$$

2p(m=0): $$\psi_{210} = \frac{1}{\sqrt{32\pi a_0^3}}\frac{r}{a_0}e^{-r/2a_0}\cos\theta$$

2p(m=±1): $$\psi_{21\pm1} = \frac{1}{\sqrt{64\pi a_0^3}}\frac{r}{a_0}e^{-r/2a_0}e^{\pm i\phi}\sin\theta$$
#### 복소수 파동함수 표

|  n  |  l  |  m  | 파동함수 $\psi_{nlm}(r,\theta,\phi)\quad\quad\quad\quad\quad\quad\quad$        |
| :-: | :-: | :-: | :------------------------------------------------------------------------- |
|  1  |  0  |  0  | $\frac{1}{\sqrt{\pi a_0^3}}e^{-r/a_0}$                                     |
|  2  |  0  |  0  | $\frac{1}{\sqrt{32\pi a_0^3}}\left(2-\frac{r}{a_0}\right)e^{-r/2a_0}$      |
|  2  |  1  |  0  | $\frac{1}{\sqrt{32\pi a_0^3}}\frac{r}{a_0}e^{-r/2a_0}\cos\theta$           |
|  2  |  1  | +1  | $\frac{1}{\sqrt{64\pi a_0^3}}\frac{r}{a_0}e^{-r/2a_0}e^{i\phi}\sin\theta$  |
|  2  |  1  | -1  | $\frac{1}{\sqrt{64\pi a_0^3}}\frac{r}{a_0}e^{-r/2a_0}e^{-i\phi}\sin\theta$ |
### 실수 형태
복소수 형태에서 실수 형태로의 변환은 다음과 같이 이루어진다:

2p(x): $$\psi_{2px} = \frac{1}{\sqrt{32\pi a_0^3}}\frac{r}{a_0}e^{-r/2a_0}\sin\theta\cos\phi$$

2p(y): $$\psi_{2py} = \frac{1}{\sqrt{32\pi a_0^3}}\frac{r}{a_0}e^{-r/2a_0}\sin\theta\sin\phi$$

이는 복소수 형태의 선형 결합으로 얻어진다:
$$\psi_{2px} = \frac{1}{\sqrt{2}}(\psi_{211} + \psi_{21-1})$$
$$\psi_{2py} = \frac{i}{\sqrt{2}}(\psi_{211} - \psi_{21-1})$$

### 실수 파동함수 표

|  n  |  l  |  오비탈   | 파동함수 $\psi_{nl}(r,\theta,\phi)\quad\quad\quad\quad\quad\quad\quad$       |
| :-: | :-: | :----: | :----------------------------------------------------------------------- |
|  1  |  0  |   1s   | $\frac{1}{\sqrt{\pi a_0^3}}e^{-r/a_0}$                                   |
|  2  |  0  |   2s   | $\frac{1}{\sqrt{32\pi a_0^3}}\left(2-\frac{r}{a_0}\right)e^{-r/2a_0}$    |
|  2  |  1  | 2p$_z$ | $\frac{1}{\sqrt{32\pi a_0^3}}\frac{r}{a_0}e^{-r/2a_0}\cos\theta$         |
|  2  |  1  | 2p$_x$ | $\frac{1}{\sqrt{32\pi a_0^3}}\frac{r}{a_0}e^{-r/2a_0}\sin\theta\cos\phi$ |
|  2  |  1  | 2p$_y$ | $\frac{1}{\sqrt{32\pi a_0^3}}\frac{r}{a_0}e^{-r/2a_0}\sin\theta\sin\phi$ |

### 데카르트 좌표계로의 변환
구면 좌표계에서 데카르트 좌표계로의 변환은 다음 관계를 이용한다:

$$x = r\sin\theta\cos\phi$$
$$y = r\sin\theta\sin\phi$$
$$z = r\cos\theta$$

## 원자 단위 (Atomic Units)를 이용한 파동함수

원자 단위에서는 $\hbar = m_e = e = 4\pi\epsilon_0 = 1$이며, 길이의 단위는 보어 반지름 $a_0$다. 이를 이용하면 파동함수는 더 간단한 형태로 표현된다. 예를 들어:

1s: $$\psi_{100} = \frac{1}{\sqrt{\pi}}e^{-r}$$

2s: $$\psi_{200} = \frac{1}{4\sqrt{2\pi}}(2-r)e^{-r/2}$$

2p(z): $$\psi_{210} = \frac{1}{4\sqrt{2\pi}}re^{-r/2}\cos\theta$$

이러한 표현은 계산을 간소화하고 물리적 의미를 더 명확히 드러내는 데 도움이 된다.