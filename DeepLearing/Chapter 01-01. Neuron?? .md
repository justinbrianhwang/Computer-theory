# What is a Neuron?

### Structure and Role of a Neuron

A **neuron** is the basic unit of information transmission in the **human brain**, providing the core inspiration for neural networks in artificial intelligence. Since the human brain is the ultimate learning mechanism, replicating its processes can lead to powerful results in machine learning.

---

## Biological Neuron Structure

![Neuron](https://www.hkn24.com/news/photo/201912/308456_164514_1746.jpg)

The image above shows a **biological neuron**, a cell responsible for **information processing and transmission**. The following diagram simplifies its structure:

![Neuron](https://thumb.ac-illust.com/ef/ef4a2c4692fdd0bf2eeb7a3d73da7f01_t.jpeg)

---

## Components of a Neuron

The key components of a neuron are illustrated below:

![Neuron Parts](https://i.imgur.com/OSonFsy.png)

- **Dendrite:** Receives signals from other neurons
- **Axon:** Sends signals to other neurons
- **Synapse:** The **gap** between neurons that facilitates communication

A single neuron is **useless** by itself. Much like a **single ant** can't carry heavy objects alone, a neuron must be **connected** to many other neurons to become powerful.

---

## Role of the Synapse

The **dendrite** and **axon** are not directly connected. Instead, signals pass through the **synapse**, as shown below:

![Synapse](https://upload.wikimedia.org/wikipedia/commons/1/1b/Synapse_Illustration_unlabeled.svg)

For this reason, artificial neural networks use the term **synapse** rather than dendrite or axon.

---

## Implementing a Neuron in Machines

Let’s examine the **machine representation** of a neuron:

![Artificial Neuron](https://i.imgur.com/bjaxAA2.png)

---

### Inputs and Outputs

A convenient way to think about machine neurons is as a **black box**:

- **Inputs:** Sensory data like taste, touch, and smell
- **Outputs:** Results sent as **inputs to other neurons**

Each input variable must be **standardized** and treated as an **independent variable**. Their units should be **similar in range**.

---

### Types of Output Variables

According to **statistical concepts**, the outputs can be:

- **Continuous Variables**
- **Binary Variables**
- **Categorical Variables**

For more details, refer to the [Statistics Guide](https://github.com/justinbrianhwang/Mathematics/tree/main/Introduction%20to%20Statistics).

---

### Learning Mechanism: Adjusting Weights

A machine neuron multiplies **inputs by weights**, sums them, and passes the result through an **activation function** to generate an output.

- **Weight Adjustment:** Learning is the process of adjusting **weights**.
- **Key Algorithms:**
  - **Gradient Descent:** Adjusts weights to minimize the cost function
  - **Backpropagation:** Propagates errors backward to update weights

---

## Next Step

Now that the concept of neurons is clear, let’s explore the role and types of **activation functions** in the next chapter.



# 뉴런이란? (What is a Neuron?)

### 뉴런의 구조와 역할

뉴런은 **인간의 뇌**에서 정보를 전달하는 기본 단위로, 기계 학습과 인공지능에서 신경망(Neural Network)의 영감을 제공하는 핵심 개념이다. 인간의 뇌가 최고의 학습 도구이자 학습 메커니즘이기 때문에 이를 기계적으로 재현하면 놀라운 결과를 얻을 수 있다.

---

## 인간의 뉴런 구조

![Neuron](https://www.hkn24.com/news/photo/201912/308456_164514_1746.jpg)

위 그림은 **생물학적 뉴런**의 이미지다. 뉴런은 신경계를 구성하는 기본 세포로, **정보 전달 및 처리** 역할을 한다. 아래 그림은 뉴런을 더 단순화한 도식이다.

![Neuron](https://thumb.ac-illust.com/ef/ef4a2c4692fdd0bf2eeb7a3d73da7f01_t.jpeg)

---

## 뉴런의 구성 요소

다음 그림은 뉴런의 주요 구성 요소를 설명한다:

![Neuron Parts](https://i.imgur.com/OSonFsy.png)

- **수상돌기(Dendrite):** 다른 뉴런으로부터 신호를 받는 부분
- **축삭돌기(Axon):** 신호를 전달하는 부분
- **시냅스(Synapse):** 뉴런 간 연결을 담당하는 간극

뉴런 하나만으로는 거의 쓸모가 없다. 마치 **개미 한 마리**가 짐 하나를 들 수 없는 것처럼, 수많은 뉴런이 함께 연결될 때 **강력한 연산 능력**을 발휘한다.

---

## 시냅스의 역할

축삭돌기와 수상돌기는 직접 연결되지 않고, **시냅스(Synapse)**라는 **간극(Gap)**을 통해 신호를 전달한다.

![Synapse](https://upload.wikimedia.org/wikipedia/commons/1/1b/Synapse_Illustration_unlabeled.svg)

이런 이유로, 인공 신경망에서는 **수상돌기(Dendrite)**와 **축삭돌기(Axon)**라는 용어 대신 **시냅스(Synapse)**라는 용어를 사용한다.

---

## 기계에서의 뉴런 구현

이제 **기계에서의 뉴런 모델**을 살펴보자:

![Artificial Neuron](https://i.imgur.com/bjaxAA2.png)

---

### 뉴런의 입력과 출력

기계의 뉴런을 이해하는 한 가지 방법은 **암흑 박스(Black Box)**를 상상하는 것이다:

- **입력(Input):** 미각, 촉각, 후각과 같은 **감각 정보**
- **출력(Output):** 결과가 **다른 뉴런의 입력**으로 전달

입력 변수들은 **표준화(Standardization)**되어야 하며, 각각 **독립 변수(Independent Variables)**로 취급해야 한다. 입력 값의 단위도 **비슷한 범위**여야 한다.

---

### 출력 변수의 유형

출력 값은 **통계학적 개념**에 따라 다음과 같이 분류할 수 있다:

- **연속형 변수(Continuous Variable)**
- **이진 변수(Binary Variable)**
- **범주형 변수(Categorical Variable)**

더 자세한 내용은 [통계학 자료](https://github.com/justinbrianhwang/Mathematics/tree/main/Introduction%20to%20Statistics)에서 확인할 수 있다.

---

### 학습 메커니즘: 가중치 조정

기계에서의 뉴런은 입력 값을 **가중치(Weight)**와 곱하고, 이를 합산하여 **활성화 함수(Activation Function)**에 전달해 출력을 생성한다.

- **가중치 조정:** 학습은 **가중치(Weight)**를 조정하는 과정이다.
- **사용되는 알고리즘:**
  - **Gradient Descent:** 비용 함수를 최소화하는 방향으로 가중치 조정
  - **Backpropagation:** 출력 오차를 역으로 전파해 가중치 수정

---

## 다음 단계

뉴런의 개념을 이해했으니, 다음으로 **활성화 함수(Activation Function)**의 역할과 종류에 대해 알아보자.


