# What to Learn About ANN

Below are the key concepts necessary for learning **Artificial Neural Networks (ANN)**.

---

## What is a Neuron?

A **neuron** is the **fundamental unit** of an artificial neural network. It is inspired by **biological neurons** and processes input data by applying weights and an activation function to produce an output.

### Neuron Process:
- Input signals: $x_1, x_2, ..., x_n$
- Weights: $w_1, w_2, ..., w_n$
- Bias: $b$
- Summation: $z = \sum_{i=1}^{n} w_i x_i + b$
- Activation function: $a = f(z)$

---

## What is an Activation Function?

An **activation function** determines the output of a neuron. It introduces **non-linearity**, enabling the network to learn complex patterns.

### Common Activation Functions:
1. **Sigmoid:**
   $$
   f(z) = \frac{1}{1 + e^{-z}}
   $$
   - Range: (0, 1)
   - Pros: Interpretable as probabilities
   - Cons: **Vanishing Gradient** problem

2. **ReLU (Rectified Linear Unit):**
   $$
   f(z) = \max(0, z)
   $$
   - Range: $[0, \infty)$
   - Pros: Efficient computation, mitigates vanishing gradient
   - Cons: **Dead Neuron** problem

3. **Softmax:**
   $$
   f(z_i) = \frac{e^{z_i}}{\sum_{j=1}^{n} e^{z_j}}
   $$
   - Used for multi-class classification

---

## How Does a Neural Network Work?

A neural network is organized into **layers**:
1. **Input Layer:** Receives input data
2. **Hidden Layer(s):** Performs computations using weights and biases
3. **Output Layer:** Produces the prediction result

---

## How Does a Neural Network Learn?

The **learning process** involves adjusting **weights and biases** based on input data. This process minimizes a **cost function**.

### Cost Function:
- Mean Squared Error (MSE): 
  $$
  J(\theta) = \frac{1}{m} \sum_{i=1}^{m} (y_i - \hat{y}_i)^2
  $$

---

## Gradient Descent

**Gradient Descent** is an algorithm that finds the **minimum** of a cost function by following its **gradient**.

---

## Stochastic Gradient Descent

**Stochastic Gradient Descent (SGD)** updates weights after evaluating the cost for **one data sample** at a time.

---

## Backpropagation Algorithm

The **Backpropagation Algorithm** adjusts weights and biases by **propagating the error backward** from the output layer to the input layer.

---

These key concepts provide a strong foundation for understanding **Artificial Neural Networks (ANNs)**.


# ANN에서 배울 것

다음은 **인공신경망(ANN)**을 학습하기 위해 필수적으로 알아야 할 주요 개념들이다.

---

## 뉴런이란?

뉴런은 **인공신경망의 기본 단위**다. 이는 **생물학적 뉴런**에서 영감을 받아 만들어진 개념으로, 입력 값을 받아 가중치를 적용하고, 활성화 함수를 통해 출력 값을 생성한다.

### 뉴런 동작 과정:
- 입력 신호 $x_1, x_2, ..., x_n$
- 가중치 $w_1, w_2, ..., w_n$
- 바이어스 $b$
- 총합(Sum): $z = \sum_{i=1}^{n} w_i x_i + b$
- 활성화 함수 적용: $a = f(z)$

---

## 활성화 함수란?

활성화 함수는 뉴런의 출력을 결정하는 함수다. **비선형성(Non-linearity)**을 부여하여 복잡한 패턴을 학습할 수 있게 해준다.

### 주요 활성화 함수:
1. **시그모이드(Sigmoid):**
   $$
   f(z) = \frac{1}{1 + e^{-z}}
   $$
   - 값 범위: (0, 1)
   - 장점: 확률적 해석 가능
   - 단점: **기울기 소실(Vanishing Gradient)** 문제 발생

2. **ReLU(Rectified Linear Unit):**
   $$
   f(z) = \max(0, z)
   $$
   - 값 범위: $[0, \infty)$
   - 장점: 계산 효율이 높고, 기울기 소실 문제 완화
   - 단점: **죽은 뉴런(Dead Neuron)** 문제 발생 가능

3. **소프트맥스(Softmax):**
   $$
   f(z_i) = \frac{e^{z_i}}{\sum_{j=1}^{n} e^{z_j}}
   $$
   - 다중 클래스 분류에서 사용

---

## Neural Network의 작동방식

뉴럴 네트워크는 **계층 구조**로 이루어져 있다:
1. **입력층(Input Layer):** 데이터를 입력받는 계층
2. **은닉층(Hidden Layer):** 가중치와 바이어스를 통해 계산을 수행하는 계층
3. **출력층(Output Layer):** 예측 결과를 출력하는 계층

### 동작 원리:
1. 입력 데이터를 각 뉴런에 전달한다.
2. 각 뉴런은 가중치와 바이어스를 적용하고 활성화 함수를 통해 출력을 생성한다.
3. 출력을 다음 계층으로 전달한다.
4. 마지막 계층에서 최종 출력을 계산한다.

---

## Neural Network가 어떻게 학습하느냐?

**학습 과정**은 주어진 데이터를 기반으로 **가중치와 바이어스**를 조정하는 과정이다. 이 과정은 **비용 함수(Cost Function)**를 최소화하는 방향으로 진행된다.

### 비용 함수(Cost Function):
- 평균 제곱 오차(MSE): 
  $$
  J(\theta) = \frac{1}{m} \sum_{i=1}^{m} (y_i - \hat{y}_i)^2
  $$

---

## Gradient Descent

**경사 하강법(Gradient Descent)**은 **비용 함수의 기울기(Gradient)**를 따라 **최소값(Minimum)**을 찾는 알고리즘이다.

### 경사 하강법 공식:
- 가중치 업데이트: 
  $$
  w := w - \alpha \frac{\partial J}{\partial w}
  $$
- 학습률 $\alpha$: 학습 속도를 조절하는 값

---

## 확률적 Gradient Descent

**확률적 경사 하강법(SGD)**은 매번 **하나의 데이터 샘플**에 대해 비용 함수를 계산하고 가중치를 업데이트하는 방식이다.

### 특징:
- 빠르게 학습 가능
- 잡음이 많아 최적해 근처에서 진동 가능

---

## Backpropagation Algorithm

**역전파 알고리즘(Backpropagation Algorithm)**은 신경망 학습에서 **오차(Error)**를 **출력층에서 입력층으로 전파**하며 **가중치와 바이어스**를 조정하는 알고리즘이다.

### 주요 단계:
1. **순방향 전파(Forward Propagation):** 예측 결과 생성
2. **오차 계산(Error Calculation):** 예측 값과 실제 값 비교
3. **역방향 전파(Backward Propagation):** 오차를 역방향으로 전파하여 기울기 계산
4. **가중치 업데이트(Weight Update):** 경사 하강법을 사용해 가중치와 바이어스 업데이트
