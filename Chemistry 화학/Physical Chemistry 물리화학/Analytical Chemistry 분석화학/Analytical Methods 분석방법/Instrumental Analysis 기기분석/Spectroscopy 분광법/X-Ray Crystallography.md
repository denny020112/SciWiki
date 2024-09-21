---
aliases:
  - X-ray crystallography
  - 엑스선 결정학
category:
  - 구조분석
  - 물리화학
related_concepts:
  - 회절
  - 브래그 법칙
  - 결정구조
tags:
  - 분자구조
  - 단결정
  - 회절패턴
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
# X선 결정학

## 정의
X선 결정학은 결정화된 물질에 X선을 조사하여 얻은 회절 패턴을 분석함으로써 물질의 원자 및 분자 구조를 결정하는 기술이다.

## 핵심 원리
1. X선의 회절
2. 브래그 법칙
3. 전자밀도 맵 계산
4. 구조 정제

## 상세 설명
X선 결정학은 물질의 결정 구조에 X선을 조사할 때 발생하는 회절 현상을 이용한다. 결정 내 원자들의 주기적 배열로 인해 특정 방향으로 X선이 강하게 회절되며, 이 회절 패턴을 분석하여 원자의 3차원 배열을 결정할 수 있다.

브래그 법칙(nλ = 2d sinθ)은 X선 회절의 기본 원리를 설명한다. 여기서 n은 정수, λ는 X선의 파장, d는 결정면 사이의 간격, θ는 입사각이다.

회절 데이터로부터 전자밀도 맵을 계산하고, 이를 바탕으로 분자 모델을 구축한다. 이후 구조 정제 과정을 통해 최종적인 분자 구조를 결정한다.

## 수학적 표현
### 브래그 법칙:
$$n\lambda = 2d \sin\theta$$

### 구조 인자 (Structure factor):
$$F_{hkl} = \sum_{j=1}^{N} f_j e^{2\pi i (hx_j + ky_j + lz_j)}$$

여기서 f<sub>j</sub>는 원자 산란 인자, (x<sub>j</sub>, y<sub>j</sub>, z<sub>j</sub>)는 원자의 좌표다.

## 적용 예시
- 예시 1: DNA 이중 나선 구조 결정 (Watson & Crick, 1953)
- 예시 2: 단백질의 3차원 구조 분석
- 예시 3: 신약 개발을 위한 단백질-리간드 상호작용 연구

## 역사적 배경
X선 결정학은 1912년 Max von Laue가 결정을 통과한 X선의 회절 현상을 발견하면서 시작되었다. 1913년 William Henry Bragg와 그의 아들 William Lawrence Bragg가 브래그 법칙을 발표하며 이론적 기반을 마련했다.

## 실험적 증거
1. NaCl 결정 구조 결정 (Bragg, 1913)
2. 단백질 구조 결정 (Myoglobin, Kendrew et al., 1958)
3. 리보솜 구조 분석 (Yonath et al., 2000)

## 한계와 예외
- 결정화가 어려운 물질에는 적용 불가능
- 수소 원자의 위치 결정이 어려움
- 동적인 구조 변화 관찰의 한계

## 관련 개념
- [[회절]]
- [[브래그 법칙]]
- [[결정구조]]
- [[푸리에 변환]]

## 응용 분야
- 구조 생물학
- 재료 과학
- 무기 화학
- 유기 화학
- 광물학

## 최근 연구 동향
- 시간 분해 X선 결정학을 통한 동적 구조 연구
- 마이크로 전자빔 회절을 이용한 나노 결정 분석
- 자유 전자 레이저를 이용한 초고속 결정학

## 학습 팁
- 결정학 기하학과 대칭성 개념 이해
- 푸리에 변환의 원리 학습
- 실제 회절 데이터 처리 및 해석 연습

## 연습 문제
1. 브래그 법칙을 이용하여 결정면 간격을 어떻게 계산할 수 있는가?
2. 구조 인자(Structure factor)의 의미와 중요성을 설명하시오.
3. X선 결정학에서 위상 문제(phase problem)란 무엇이며, 어떻게 해결하는가?

## 참고문헌
1. Rupp, B. (2009). Biomolecular Crystallography: Principles, Practice, and Application to Structural Biology. Garland Science.
2. Giacovazzo, C. et al. (2011). Fundamentals of Crystallography (3rd ed.). Oxford University Press.

## 추가 노트
X선 결정학은 20세기 과학의 가장 중요한 발견들 중 많은 부분에 기여했다. DNA 구조 발견부터 단백질 구조 연구에 이르기까지, 생명 과학의 발전에 핵심적인 역할을 했다. 현재도 신약 개발, 재료 과학 등 다양한 분야에서 중요하게 활용되고 있다.