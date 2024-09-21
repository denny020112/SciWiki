---
aliases:
  - 핵자기공명
  - Nuclear Magnetic Resonance
  - NMR
category:
  - 분석법
  - 구조
related_concepts:
  - IR 분광법
  - 질량 분석법
tags:
  - 분광학
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
# 핵자기공명 분광법 (NMR)
## 정의 및 개요

1946년 Bloch와 Purcell이 NMR 현상을 발견했으며, 1950년대부터 화학 구조 분석에 활용되기 시작했다. 이후 초전도 자석과 푸리에 변환 기술의 도입으로 감도가 크게 향상되었다.
핵자기공명 분광법(Nuclear Magnetic Resonance, NMR)은 강한 자기장 내에서 특정 원자핵의 공명 주파수를 측정하여 분자 구조를 분석하는 분광학적 기술이다. 주로 유기화합물의 구조 결정에 사용된다.


## 상세 원리

### 핵 스핀 상태 (Nuclear Spin States)

특정 원자핵(주로 <sup>1</sup>H, <sup>13</sup>C)은 고유한 스핀을 가진다. 이 스핀은 자기장 내에서 특정 에너지 준위로 나뉜다.

#### 핵 자기 모멘트 (Nuclear Magnetic Moment)

스핀을 가진 핵은 자기 모멘트를 갖게 되며, 이는 외부 자기장과 상호작용한다.

### 에너지 흡수와 그 메커니즘

핵은 특정 주파수의 전자기파를 흡수하여 낮은 에너지 상태에서 높은 에너지 상태로 전이할 수 있다.

##### 차폐 효과 (Shielding effect)

전자들이 핵 주위를 순환하면서 작은 국소 자기장을 만들어 외부 자기장을 차폐한다. 이를 차폐 효과(shielding effect)라고 한다.

###### 주파수 식 유도 

$$\nu = \frac{\gamma}{2\pi}(B_o - B_{local})$$

여기서 $\nu$는 공명 주파수, $\gamma$는 자기회전비(magnetogyric ration), $B_o$는 외부 자기장, $B_{local}$은 국소 자기장이다.

##### 화학적 이동

서로 다른 화학적 환경에 있는 핵들은 서로 다른 정도로 차폐되어 다른 공명 주파수를 갖게 된다. 이 차이를 화학적 이동(chemical shift)이라 한다.

- TMS(테트라메틸실란)가 기준(0 ppm)으로 사용된다. 
	- TMS의 양성자들은 거의 모든 유기 화합물의 양성자보다 더 차폐되어 있기 때문이다.
	- TMS는 대부분의 유기 용매에 녹는다. 
- 다운필드: TMS보다 높은 주파수(낮은 자기장)에서 공명
- 업필드: TMS보다 낮은 주파수(높은 자기장)에서 공명

화학적 이동 (δ) = (ν - νref) / νref × 106 ppm
여기서 ν는 측정된 공명 주파수, νref는 기준물질(TMS)의 공명 주파수이다.
###### 화학적 이동 식 유도

$$\delta = \frac{frequency (Hz) - frequency TMS (Hz)}{frequency TMS (MHz)}$$

화학적 이동은 ppm 단위로 표시되는데, 이는 측정 장비의 자기장 세기에 무관한 값을 얻기 위함이다.


### 탈차폐 요인 (Deshielding Factors)

다음 요인들이 핵의 차폐를 감소시켜(deshielding) 화학적 이동값을 증가시킨다:

#### 수소 결합

수소 결합은 전자 밀도를 감소시켜 양성자를 더 deshield한다.

#### 오비탈 혼성 (Hybridization)

sp > sp<sup>2</sup> > sp<sup>3</sup> 순으로 s 성격이 증가하여 deshielding 효과가 커진다.

#### 자기 이방성 (Magnetic Anisotropy)

이중결합이나 방향족 고리의 π 전자들이 만드는 환전류에 의해 특정 위치의 양성자들이 deshield된다.

#### 전기음성도 효과 (Electronegativity Effect)

전기음성도가 큰 원자가 인접해 있으면 전자를 끌어당겨 해당 양성자를 deshield한다.

## NMR 스펙트럼 해석

- 자연 존재비가 낮은 동위원소(13C 등)의 경우 감도가 낮다.
- 상자성 물질이 존재하면 스펙트럼 해석이 어려워진다.
- 매우 빠른 분자 운동이 있는 경우 신호가 평균화될 수 있다.
### 화학적 등가성 (Chemical Equivalence)

화학적으로 동등한(equivalent) 핵들은 동일한 화학적 이동 (chemical shift)를 갖는다.

### 커플링 상수, J (Coupling constant)

커플링 상수는 인접한 핵들 간의 상호작용 강도를 나타내며, 스펙트럼에서 신호가 분리되는 정도를 Hz 단위로 측정한 값이다.

#### 커플링 상수 식 유도 (Coupling Constant Equation Derivation)

두 개의 인접한 스핀-1/2 핵 (A와 X)에 대해:

$$J_{AX} = \frac{1}{2}(\nu_1 - \nu_2) = \frac{1}{2}(\nu_3 - \nu_4)$$

여기서 $\nu_1$, $\nu_2$, $\nu_3$, $\nu_4$는 AX 스핀 시스템의 네 가지 전이 주파수다.

커플링 상수는 화학적 이동과 달리 자기장 세기에 무관하며, 결합 각도나 결합 거리 등 분자 구조에 대한 정보를 제공한다.

### <sup>1</sup>H NMR

가장 널리 사용되는 NMR 기법으로, 양성자의 공명을 관찰한다.
#### 피크의 갯수

- 스플리팅 (n+1 규칙; 멀티플렛): 인접한 양성자의 수에 따라 신호(signal)가 n+1개로 갈라진다.
#### 피크의 면적 (integration)

해당하는 양성자의 갯수를 알려줌
#### 화학적 이동



### <sup>13</sup>C NMR

탄소-13 동위원소의 공명을 관찰한다.

#### 양성자 커플링 (proton coupling)

<sup>13</sup>C-<sup>1</sup>H 커플링으로 인해 복잡한 스펙트럼이 생성될 수 있다.

#### 양성자 디커플링(proton decoupling)

양성자와의 커플링을 제거하여 단순화된 스펙트럼을 얻는 기술이다.

#### Nuclear Overhauser Enhancement (NOE)

양성자 decoupling 과정에서 <sup>13</sup>C signal의 강도가 증가하는 현상이다.
#### 화학적 이동
탄소 원자의 혼성 상태와 주변 원자의 영향을 반영한다.

- sp<sup>3</sup> 탄소: 0-50 ppm
- sp<sup>2</sup> 탄소: 100-150 ppm
- sp 탄소: 65-85 ppm
- 카보닐 탄소: 160-220 ppm


### <sup>19</sup>F NMR

불소 화합물 분석에 유용하다.

### <sup>31</sup>P NMR

유기인 화합물 분석에 사용된다.

## 응용 분야
- 유기 화합물의 구조 결정
- 단백질 구조 분석
- 신약 개발 과정의 화합물 분석
- 대사체학 연구
- MRI 의료 영상

## 관련 개념
- [[IR Spectroscopy|IR 분광법]]
- [[SciWiki/Chemistry 화학/Physical Chemistry 물리화학/Analytical Chemistry 분석화학/Analytical Methods 분석방법/Instrumental Analysis 기기분석/Mass Spectrometry|질량 분석법]]
- [[X-Ray Crystallography|X선 결정학]]



## 참고문헌

1. Silverstein, R. M. et al. Spectrometric Identification of Organic Compounds, 8th ed.; Wiley, 2014.
2. Keeler, J. Understanding NMR Spectroscopy, 2nd ed.; Wiley, 2010.
3. Claridge, T. D. W. High-Resolution NMR Techniques in Organic Chemistry, 3rd ed.; Elsevier, 2016.

