---
aliases:
  - 유전율
category:
  - 물리학
related_concepts:
  - 전기장
  - 전하
tags:
  - 전자기학
  - 물리
  - 전기
---

```table-of-contents
title: 
style: nestedList # TOC style (nestedList|nestedOrderedList|inlineFirstLevel)
minLevel: 0 # Include headings from the specified level
maxLevel: 0 # Include headings up to the specified level
includeLinks: true # Make headings clickable
debugInConsole: false # Print debug info in Obsidian console
```
# 유전율 (Permittivity)
![[dielectric internal Efield (permittivity).png]]
## 정의
유전율 (誘電率)은 전기장에 노출된 물질[^1]의 전기에너지를 저장하는 능력, 즉 전기장에 의해 물체 내부의 전하가 편극되는 정도를 뜻한다. 더 쉽게 설명하자면, 물질 내에서 전하가 얼마나 쉽게 재배열되는지 나타낸다. 높은 유전율은 강한 편극 정도를 의미하며 이는 약한 내부 전기장으로 이어진다. 수학적 표현은 아래와 같다:

$$E_{internal} = E_{external} - E_{polarization} = E_{external} - \frac{P}{\varepsilon_0}$$
단, 얼만큼 전하가 잘 *흐르는지를* 의미하는 것은 아니다. 전하가 흐르는 순간 더이상 전하의 편극이 아니라 [[Electric Current|전류(electric current)]]로 간주되기 때문이다.

### 편극 (Polarisation)
![[electric polarisation.png|400]]
편극이란 외부의 전기장에 의해 전하가 한쪽으로 쏠리는 현상이다. 
$$\mathbf{P}=\epsilon_{0}\chi_{e}\mathbf{E}$$
- $\mathbf{P}$, 편극(polarisation) 벡터
- $\epsilon_{0}$, 진공 유전율 (vacuum permittivity); 약 $8.85 \times 10^{-12}$ F/m
- $\chi_{e}$, 전기 감수율 (electric susceptibility)
- $\mathbf{E}$, 외부 전기장 (external electric field)





[^1]: 대체로 [[Dielectric|유전체(dielectric material)]]을 의미한다