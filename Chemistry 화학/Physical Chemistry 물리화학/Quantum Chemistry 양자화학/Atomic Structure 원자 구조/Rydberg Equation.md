---
aliases:
  - Rydberg formula
  - 뤼드베리 방정식
  - 리드버그 방정식
category:
  - 원자물리학
  - 분광학
related_concepts:
  - 보어 모델
  - 수소 원자 스펙트럼
  - 에너지 준위
tags:
  - 양자화
  - 화학
  - 물리
  - 양자화학
  - 원자구조
  - 분광학
---

```table-of-contents
title: 
style: nestedList # TOC style (nestedList|nestedOrderedList|inlineFirstLevel)
minLevel: 0 # Include headings from the specified level
maxLevel: 0 # Include headings up to the specified level
includeLinks: true # Make headings clickable
debugInConsole: false # Print debug info in Obsidian console
```

# 뤼드베리 공식 (Rydberg Equation)

## 정의
뤼드베리 공식은 원자의 스펙트럼 선을 설명하는 경험적 공식으로, 특히 수소와 수소 유사 원자의 스펙트럼 선 파장을 정확히 예측한다.

## 공식

### 기본 공식
뤼드베리 공식의 가장 기본적인 형태는 다음과 같다:

$$ \frac{1}{\lambda} = R_H (\frac{1}{n_1^2} - \frac{1}{n_2^2}) $$

여기서:
- $\lambda$: 방출 또는 흡수되는 빛의 파장
- $R_H$: 뤼드베리 상수 (수소의 경우 1.097 × 10^7 m^-1)
- $n_1, n_2$: 양자수 ($n_2 > n_1$)



### 에너지 관점의 공식

에너지 관점에서 뤼드베리 공식은 다음과 같이 표현된다:

$$ \Delta E = E_2 - E_1 = R_H hc (\frac{1}{n_1^2} - \frac{1}{n_2^2}) $$

여기서:
- $\Delta E$: 에너지 차이
- $h$: 플랑크 상수
- $c$: 빛의 속도

### 일반화된 뤼드베리 공식
다전자 원자나 이온에 대해 일반화된 형태는 다음과 같다:

$$ \frac{1}{\lambda} = R_Z (\frac{1}{n_1^2} - \frac{1}{n_2^2}) $$

여기서 $R_Z$는 원자 번호 Z에 대한 수정된 뤼드베리 상수:

$$ R_Z = R_\infty \frac{\mu}{m_e} $$

- $R_{\infty}$: 무한대 질량 뤼드베리 상수
- μ: 핵과 전자의 환산 질량 (Reduced mass)
- $m_e$: 전자 질량


## 계산 예시 
### 예시 1: 수소 원자의 발머 계열 
발머 계열은 n₁ = 2일 때의 전이를 나타낸다. n₂ = 3에서 n₁ = 2로의 전이를 계산해보자. 
$$ \frac{1}{\lambda} = R_H (\frac{1}{n_1^2} - \frac{1}{n_2^2}) $$ $$ \frac{1}{\lambda} = 1.097 \times 10^7 m^{-1} (\frac{1}{2^2} - \frac{1}{3^2}) $$ $$ \frac{1}{\lambda} = 1.097 \times 10^7 m^{-1} (0.25 - 0.1111) $$ $$ \frac{1}{\lambda} = 1.524 \times 10^6 m^{-1} $$ $$ \lambda = 6.563 \times 10^{-7} m = 656.3 nm $$ 이는 수소 원자 스펙트럼의 붉은색 선에 해당한다. 
### 예시 2: 에너지 준위 차이 계산 
n₁ = 1에서 n₂ = 2로의 전이에 대한 에너지 차이를 계산해보자. $$ \Delta E = R_H hc (\frac{1}{n_1^2} - \frac{1}{n_2^2}) $$ 여기서: - R_H = 1.097 × 10^7 m^-1 - h = 6.626 × 10^-34 J·s - c = 2.998 × 10^8 m/s $$ \Delta E = (1.097 \times 10^7)(6.626 \times 10^{-34})(2.998 \times 10^8) (\frac{1}{1^2} - \frac{1}{2^2}) $$ $$ \Delta E = 2.179 \times 10^{-18} J (1 - 0.25) $$ $$ \Delta E = 1.634 \times 10^{-18} J $$ 이를 전자볼트(eV)로 변환하면: $$ \Delta E = 10.2 eV $$ 이는 수소 원자의 첫 번째 들뜬 상태에서 기저 상태로의 전이 에너지에 해당한다. 
### 예시 3: 헬륨 이온 (He⁺)의 스펙트럼 선 계산
He⁺는 수소와 유사한 원자로, 수정된 뤼드베리 상수를 사용해야 한다. He⁺의 경우 Z = 2이므로: $$ R_{He^+} = R_H Z^2 = (1.097 \times 10^7 m^{-1})(2^2) = 4.388 \times 10^7 m^{-1} $$ n₁ = 2에서 n₂ = 3으로의 전이를 계산해보자: $$ \frac{1}{\lambda} = 4.388 \times 10^7 m^{-1} (\frac{1}{2^2} - \frac{1}{3^2}) $$ $$ \frac{1}{\lambda} = 6.094 \times 10^6 m^{-1} $$ $$ \lambda = 1.641 \times 10^{-7} m = 164.1 nm $$ 이는 He⁺ 이온의 자외선 영역 스펙트럼 선에 해당한다.
## 역사적 배경
- 1888년: 요하네스 뤼드베리가 경험적으로 공식 제안
- 1913년: 닐스 보어의 원자 모델로 이론적 근거 제공

## 스펙트럼 계열

![[hydrogen spectra series.png]]

수소 스펙트럼에서 바닥 상태의 주양자수(n)에 따라 결정된다.

1. 라이먼 계열 (n_1 = 1)
2. 발머 계열 (n_1 = 2)
3. 파셴 계열 (n_1 = 3)
4. 브라켓 계열 (n_1 = 4)
5. 푼트 계열 (n_1 = 5)

## 관련 개념
- 보어 모델
- 양자화된 에너지 준위
- 선 스펙트럼
- 진동수 조건

## 참고문헌
1. Griffiths, D. J. (2004). Introduction to Quantum Mechanics. Pearson Prentice Hall.
2. Herzberg, G. (1944). Atomic Spectra and Atomic Structure. Dover Publications.
3. Bethe, H. A., & Salpeter, E. E. (1957). Quantum Mechanics of One- and Two-Electron Atoms. Springer-Verlag.