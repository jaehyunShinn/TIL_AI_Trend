# 1. VGLM (Vector Generalized Linear Model)

## 1.1 개요
VGLM은 GLM(Generalized Linear Model)의 확장 모델로,  
여러 개의 반응변수(출력)를 동시에 모델링할 수 있도록 설계된 통계적 프레임워크이다.

기존 GLM:
g(E[Y]) = X * beta

VGLM:
g(E[Y_vector]) = X * B

- Y_vector: 다차원 출력 벡터
- X: 설명변수 행렬
- B: 계수 행렬
- g(): 링크 함수

즉, 하나의 입력으로 여러 출력을 동시에 학습하는 모델이다.

---

## 1.2 GLM vs VGLM

| 구분 | GLM | VGLM |
|------|-----|------|
| 출력 | 스칼라 | 벡터 |
| 모델링 | 단일 반응변수 | 다중 반응변수 |
| 구조 | \( X\beta \) | \( X\mathbf{B} \) |
| 목적 | 단일 예측 | 멀티태스크 예측 |

---

## 1.3 수학적 구조

### (1) 단일 출력 GLM


### (2) 다중 출력 VGLM


각 출력 차원마다 서로 다른 계수 벡터를 갖는다.

## 1.4 링크 함수
VGLM은 각 출력 차원마다 다양한 링크 함수를 사용할 수 있다.

- Logistic link → 확률 예측
- Log link → count 데이터
- Identity link → 연속값 예측
- Softmax link → 다중 클래스 확률 벡터

특히 Softmax 기반 구조는 다중 클래스 분류 모델과 구조적으로 유사하다.

---

## 1.5 머신러닝 관점 해석
VGLM은 선형 모델 기반의 멀티태스크 학습으로 해석할 수 있다.

Y_hat = X * W

이는 신경망에서 마지막 선형 레이어와 유사하며,  
여러 개의 타겟을 동시에 예측하는 구조를 가진다.
