---
aliases:
  - IR spectroscopy
  - 적외선 분석법
category:
  - 분석화학
  - 분광학
related_concepts:
  - 진동 분광학
  - 푸리에 변환 적외선 분광법
  - 라만 분광법
tags:
  - 유기화학
  - 분광학
  - 분석화학
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

# 적외선 분광법 (Infrared Spectroscopy)

## 정의 및 개요

적외선에 의한 분자의 진동 에너지 준위 사이의 전이를 이용하여 분자 구조를 분석하는 분광학적 방법이다. 

## 상세 설명

거시세계가 아닌 미시세계에서의 에너지는 양자화되어있음을 고려하여 생각해야 한다.
적외선의 경우에는 고에너지 전자기파가 아니기 때문에 분자의 진동에 영향을 주는 것 정도 밖에는 할 수 없다.

특정 준위에 맞는 에너지만 방출 혹은 흡수되기 때문에 시료에 적외선을 가했을 때 분자 고유의 진동수에 알맞은  파장 혹은 진동수만 흡수된다. 이는 분자 내 결합의 진동의 크기(amplitude)를 증가시키며, 진동의 빈도에는 영향을 주지 않는다.

적외선 분광학에서는 각 분자가 흡수하는 고유의 진동수, 그리고 각 작용기가 흡수하는 고유의 진동수를 활용하여 분자의 구조와 작용기를 식별하는 것을 목적으로 한다.

### 분자의 진동

![[modes of molecular vibration.png|450]]


분자의 진동은 크게 다음과 같은 종류로 나눌 수 있다:

1. 신축 진동 (Stretching vibration). 
	결합의 축에서 일어나는 진동을 의미한다. 
	- 대칭 신축 (Symmetric stretching): 결합 길이가 동시에 늘어나거나 줄어듦
	- 비대칭 신축 (Asymmetric stretching): 한 결합은 늘어나고 다른 결합은 줄어듦

2. 굽힘 진동 (Bending vibration)
	- 면내 굽힘 (In-plane bending)
	    - 가위질 (Scissoring): 결합각이 커졌다 작아짐
	    - 흔들림 (Rocking): 결합각은 유지한 채 전체가 흔들림
	- 면외 굽힘 (Out-of-plane bending)
	    - 꼬임 (Twisting): 평면에서 벗어나 비틀림
	    - 흔들림 (Wagging): 평면에서 벗어나 흔들림

3. 비틀림 진동 (Torsional vibration)
	- 두 평면 사이의 이면각이 변화함

또한 진동은 분자의 구조와 대칭성에 따라 다르게 나타난다. 예를 들어:
- 이원자 분자: 신축 진동만 가능
- 삼원자 분자: 선형이면 4개, 굽은 형태면 3개의 진동 모드 존재
- 더 복잡한 분자[^1]: 3N-6개(선형 분자는 3N-5개)의 진동 모드 존재

단, 적외선에 의한 분자 진동의 증폭은 분자가 극성 모멘트를 가지고 있을 때에만 발생하기 때문에 비극성 결합으로만 이루어진 분자 혹은 대칭성을 지닌 분자는 적외선 분광으로 분석하는데 애로 사항이 따른다. 


## 적외선 분광 해석

![[ir spectrum.png]]

적외선의 영역은 400~4000 $\text{cm}^{-1}$ 이다. 이 영역은 다음과 같이 3 영역으로 나눌 수 있다.

1. 근적외선 (NIR): 14000-4000 $\text{cm}^{-1}$
2. 중적외선 (MIR): 4000-400 $\text{cm}^{-1}$ (가장 일반적으로 사용)
3. 원적외선 (FIR): 400-10 $\text{cm}^{-1}$

주로 작용기의 영역은 근적외선 부근인 4000~1500 $\text{cm}^{-1}$ 에서 나타나며, 
분자의 고유 구조[^2]를 나타내는 영역은 1500-400 $\text{cm}^{-1}$에서 나타난다. 

### 스펙트럼 해석

1. 작용기 영역 (4000-1500 cm^-1^): 특정 작용기 식별
2. 지문 영역 (1500-400 cm^-1^): 분자의 고유 패턴

진동 주파수는 결합의 강도와 원자 질량에 의존한다.
결합의 세기가 강하고 그 길이가 짧을 때에 더 높은 진동수를 보여준다.
또한 결합이 극성도가 강하면 강할 수록 더 강한 피크가 나타난다.

x축: 파수 ($\text{cm}^{-1}$), y축: 투과도(%) 또는 흡광도

### 구조 해석

![[fx gorup and fingerprint.png|450]]
지문영역의 경우에는 작용기만을 보는 것 보다 복잡할 수 있기 때문에 유의해야한다. 
- 개별 밴드의 해석보다는 전체적인 패턴을 보는 것이 중요
- 복잡한 패턴으로 인해 개별 밴드 할당이 어려울 수 있음
- 동위원소 치환에 의해 밴드 위치가 변할 수 있음

#### 주요  흡수 밴드

- O-H 신축: 3200-3600 $\text{cm}^{-1}$
- C-H 신축: 2850-3000 $\text{cm}^{-1}$
- C=O 신축: 1670-1820 $\text{cm}^{-1}$
- C=C 신축: 1620-1680 $\text{cm}^{-1}$
- C-O 신축: 1000-1300 $\text{cm}^{-1}$
- C-N 신축: 1350-1000 $\text{cm}^{-1}$
- C-X[^3] 신축: 850-500 $\text{cm}^{-1}$
- 방향족 C-H 면외 굽힘: 900-690 $\text{cm}^{-1}$
#### 작용기별 특징

- [[alcohol|알코올]]: O-H 신축 (3400-3200 $\text{cm}^{-1}$), C-O 신축 (1260-1050 $\text{cm}^{-1}$)
- 카르복실산: O-H 신축 (3300-2500 $\text{cm}^{-1}$, 매우 넓음), C=O 신축 (1720-1700 $\text{cm}^{-1}$)
- [[Ester|에스터]]: C=O 신축 (1750-1735 $\text{cm}^{-1}$), C-O 신축 (1300-1000 $\text{cm}^{-1}$)
- 아민: N-H 신축 (3500-3300 $\text{cm}^{-1}$, 두 개의 밴드)
- 알데하이드: C-H 신축 (2850-2820 $\text{cm}^{-1}$), C=O 신축 (1740-1720 $\text{cm}^{-1}$)


## 장치 구성
1. 광원: 글로바 또는 Nernst 필라멘트
2. 단색화 장치: 프리즘 또는 회절격자
3. 시료 홀더
4. 검출기: 열전대 또는 열전지

## 시료 준비 방법
1. KBr 펠릿
2. 용액 셀
3. ATR (감쇠 전반사)
4. 기체 셀

## 장단점
장점:
- 비파괴적 분석
- 다양한 시료 형태 분석 가능
- 빠른 분석 속도

단점:
- 수분에 민감
- 무기 화합물 분석에 제한적
- 복잡한 혼합물 분석 어려움

## 추가 노트

적외선 분광법은 유기 화합물의 구조 분석에 매우 유용하지만, 다른 분광학적 방법(예: NMR, 질량 분석)과 함께 사용할 때 가장 효과적이다.

## 관련 개념

- [[푸리에 변환 적외선 분광법]]
- [[라만 분광법]]
- [[진동 분광학]]

## 참고문헌
1. Stuart, B. (2004). Infrared Spectroscopy: Fundamentals and Applications. John Wiley & Sons.
2. Silverstein, R.M., Webster, F.X., Kiemle, D.J., Bryce, D.L. (2014). Spectrometric Identification of Organic Compounds. John Wiley & Sons.






[^1]:  N은 원자 수
[^2]: 지문 영역이라고 한다
[^3]: X(할라이드) = F, Cl, Br, I