---
aliases:
  - kinetics
  - 반응속도론
  - reaction kinetics
category:
  - 반응성
  - 유기화학 규칙
related_concepts: 
tags:
  - 유기화학
  - 알켄
  - 제거
  - 반응
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


# 화학 반응속도론

## 개요

## 반응 차수와 속도 법칙

### 0차 반응

Zeroth Order reaction

0차 반응에서 반응 속도는 반응물의 농도와 무관하다. 
즉, 시간에 대하여 농도의 변화는 선형이다.

예를 들자면, 어떠한 기체가 고체의 표면을 촉매로서 반응이 일어날 때, 고체의 면적은 제한되어있으므로 기체의 압력[^1]

속도 법칙: $$v = -\frac{d[A]}{dt} = k$$

#### 적분 형태 유도:
$$\begin{align}
-\frac{d[A]}{dt} &= k \\
-d[A] &= k \cdot dt \\
\int_{[A]_0}^{[A]} -d[A] &= \int_0^t k \cdot dt \\
-([A] - [A]_0) &= kt \\
[A] &= [A]_0 - kt
\end{align}$$

### 1차 반응

1차 반응에서 반응 속도는 반응물의 농도에 비례한다.

속도 법칙: $v = -\frac{d[A]}{dt} = k[A]$

적분 형태 유도:
$$\begin{align}
-\frac{d[A]}{dt} &= k[A] \\
-\frac{d[A]}{[A]} &= k \cdot dt \\
\int_{[A]_0}^{[A]} -\frac{d[A]}{[A]} &= \int_0^t k \cdot dt \\
-(\ln[A] - \ln[A]_0) &= kt \\
\ln[A] &= \ln[A]_0 - kt
\end{align}$$

### 2차 반응

2차 반응에서 반응 속도는 반응물 농도의 제곱에 비례한다.

속도 법칙: $v = -\frac{d[A]}{dt} = k[A]^2$

적분 형태 유도:
$$\begin{align}
-\frac{d[A]}{dt} &= k[A]^2 \\
-\frac{d[A]}{[A]^2} &= k \cdot dt \\
\int_{[A]_0}^{[A]} -\frac{d[A]}{[A]^2} &= \int_0^t k \cdot dt \\
\frac{1}{[A]} - \frac{1}{[A]_0} &= kt \\
\frac{1}{[A]} &= \frac{1}{[A]_0} + kt
\end{align}$$

## 아레니우스 식

아레니우스 식은 온도에 따른 반응 속도 상수의 변화를 나타낸다:

$$k = Ae^{-E_{a}/RT}$$

여기서 $A$는 빈도 인자, $E_a$는 활성화 에너지, $R$은 기체 상수, $T$는 절대 온도다.

### 유도
아레니우스는 반응이 일어나기 위해 분자들이 특정 에너지 장벽(활성화 에너지)을 넘어야 한다고 가정했다. 볼츠만 분포에 따라, 이 에너지 이상을 가진 분자의 비율은 에 비례한다. 따라서 반응 속도 상수는 이 비율에 비례하게 된다.

## 린데만-힌셸우드 메커니즘

린데만-힌셸우드 메커니즘은 단분자 반응의 메커니즘을 설명한다:

1. $A + A \xrightarrow{k_1} A^* + A$ (활성화)
2. $A^* \xrightarrow{k_{-1}} A + A$ (비활성화)  
3. $A^* \xrightarrow{k_2} P$ (생성물 형성)

여기서 $A^*$는 활성화된 분자를 나타낸다.

정상 상태 근사를 적용하면:

$$\begin{align}
\frac{d[A^*]}{dt} &= k_1[A]^2 - k_{-1}[A^*][A] - k_2[A^*] = 0 \\
[A^*] &= \frac{k_1[A]^2}{k_{-1}[A] + k_2}
\end{align}$$

전체 반응 속도는:

$$v = k_2[A^*] = \frac{k_1k_2[A]^2}{k_{-1}[A] + k_2}$$

고압(높은 $[A]$)에서는 $k_{-1}[A] \gg k_2$이므로:

$$v \approx \frac{k_1k_2}{k_{-1}}[A] = k_{uni}[A]$$

이는 1차 반응 속도식과 일치한다.

저압에서는 $k_2 \gg k_{-1}[A]$이므로:

$$v \approx k_1[A]^2$$

이는 2차 반응 속도식과 일치한다.

이 메커니즘은 단분자 반응의 압력 의존성을 잘 설명한다..



[^1]: 기체의 경우에는 압력이 용액에서의 농도와 비슷하게 취급된다. 기체 입자가 더 많으면 압력도 그에 비례해서 올라가기 때문이다.