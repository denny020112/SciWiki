---
aliases:
  - Fourier Transform
  - FT
  - 푸리에 급수
category:
  - 해석학
  - 신호처리
related_concepts:
  - 라플라스 변환
  - Z-변환
  - 웨이브릿 변환
tags:
  - 주파수
  - 분석
  - 신호처리
  - 적분변환
  - 수학
---

```table-of-contents
title: 
style: nestedList # TOC style (nestedList|nestedOrderedList|inlineFirstLevel)
minLevel: 0 # Include headings from the specified level
maxLevel: 0 # Include headings up to the specified level
includeLinks: true # Make headings clickable
debugInConsole: false # Print debug info in Obsidian console
```
# 푸리에 변환

## 정의

푸리에 변환은 시간 영역의 신호를 주파수 영역으로 변환하는 수학적 도구다. 연속 시간 신호 x(t)에 대한 푸리에 변환 X(f)는 다음과 같이 정의된다:

$$ X(f) = \int_{-\infty}^{\infty} x(t) e^{-j2\pi ft} dt $$

여기서 f는 주파수, t는 시간을 나타낸다.

## 중요 성질

1. 선형성: $\mathcal{F}\{ax(t) + by(t)\} = aX(f) + bY(f)$
2. 시간 이동: $\mathcal{F}\{x(t-t_0)\} = X(f)e^{-j2\pi ft_0}$
3. 주파수 이동: $\mathcal{F}\{x(t)e^{j2\pi f_0t}\} = X(f-f_0)$
4. 시간 영역 확장: $\mathcal{F}\{x(at)\} = \frac{1}{|a|}X(\frac{f}{a})$
5. 컨볼루션 정리: $\mathcal{F}\{x(t) * y(t)\} = X(f)Y(f)$


## 주요 정리

1. 파세발 정리
   증명: 파세발 정리는 시간 영역에서의 신호 에너지가 주파수 영역에서 보존됨을 나타낸다.
   $$ \int_{-\infty}^{\infty} |x(t)|^2 dt = \int_{-\infty}^{\infty} |X(f)|^2 df $$

2. 불확정성 원리
   증명: 시간과 주파수 영역에서의 신호의 폭은 서로 반비례 관계에 있다.
   $$ \Delta t \cdot \Delta f \geq \frac{1}{4\pi} $$

3. 모듈레이션 정리 (변조 정리)
   증명: 시간 영역에서의 곱셈은 주파수 영역에서의 컨볼루션과 대응한다.
   $$ \mathcal{F}\{x(t)y(t)\} = X(f) * Y(f) $$

4. 미분 정리
   증명: 시간 영역에서의 미분은 주파수 영역에서 주파수에 비례하는 곱셈과 대응한다.
   $$ \mathcal{F}\{\frac{d^n}{dt^n}x(t)\} = (j2\pi f)^n X(f) $$

5. 푸리에 변환의 유일성 정리
   증명: 두 신호의 푸리에 변환이 모든 주파수에서 동일하다면, 그 두 신호는 거의 모든 곳에서 같다.
   $$ \text{If } X_1(f) = X_2(f) \text{ for all } f, \text{ then } x_1(t) = x_2(t) \text{ almost everywhere} $$

6. 스케일링 정리
   증명: 시간 영역에서의 압축/팽창은 주파수 영역에서의 역압축/역팽창과 대응한다.
   $$ \mathcal{F}\{x(at)\} = \frac{1}{|a|}X(\frac{f}{a}) $$

7. 대칭성 정리
   증명: 푸리에 변환은 시간과 주파수 영역 사이의 대칭성을 가진다.
   $$ \text{If } \mathcal{F}\{x(t)\} = X(f), \text{ then } \mathcal{F}\{X(t)\} = x(-f) $$

## 응용

- 신호 처리
- 이미지 압축
- 통신 시스템
- 음향학
- 양자 역학

## 관련 개념

- 이산 푸리에 변환 (DFT)
- 고속 푸리에 변환 (FFT)
- 푸리에 급수
- 단시간 푸리에 변환 (STFT)

## 예제

1. 사각파의 푸리에 변환
   해설: 사각파는 무한한 개수의 사인파의 합으로 표현될 수 있으며, 이는 푸리에 변환을 통해 확인할 수 있다.

2. 가우시안 함수의 푸리에 변환
   해설: 가우시안 함수의 푸리에 변환도 가우시안 함수 형태를 가진다.

## 역사적 배경

푸리에 변환은 18세기 말 조제프 푸리에에 의해 처음 제안되었다. 그는 열전도 방정식을 풀기 위해 이 개념을 도입했으며, 이후 다양한 분야에서 응용되었다.

## 시각화

[시간 영역에서 주파수 영역으로의 변환을 나타내는 다이어그램]

## 계산 방법

1. 해석적 방법: 정의를 직접 적용하여 계산
2. 수치적 방법: 이산 푸리에 변환(DFT)을 사용
3. 고속 푸리에 변환(FFT) 알고리즘: O(N log N) 시간 복잡도로 계산 가능

## 주의사항

- 신호가 푸리에 변환의 조건(디리클레 조건)을 만족해야 한다.
- 이산 신호의 경우 앨리어싱(aliasing) 효과에 주의해야 한다.
- 윈도우 함수 선택이 스펙트럼 누설(spectral leakage)에 영향을 미친다.

## 참고 문헌

1. Oppenheim, A. V., & Schafer, R. W. (2010). Discrete-time signal processing. Pearson Higher Education.
2. Bracewell, R. N. (1986). The Fourier transform and its applications. McGraw-Hill.
3. Mallat, S. (1999). A wavelet tour of signal processing. Academic press.

## 추가 학습 자료

- MIT OpenCourseWare: Linear Systems and Signals
- Coursera: Digital Signal Processing
- YouTube: 3Blue1Brown의 푸리에 변환 시리즈