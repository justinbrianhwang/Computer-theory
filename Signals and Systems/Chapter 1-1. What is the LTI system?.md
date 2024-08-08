# English

## LTI System

LTI stands for Linear Time Invariant.

We will analyze each part of this term.

### Linear

This term can be understood in two aspects. Let's look at the first case.

**Scaling + Additivity**

First, what is scaling? It is a property where if a constant is multiplied to the input signal function, the result of the output signal function is also the same constant multiplied to it. The following diagram makes it easier to understand.

![Scaling](https://i.imgur.com/W1x0SzN.png)

Next, let's look at additivity. If the input signal is \(x_1(t)\) with the result \(y_1(t)\), and the input signal is \(x_2(t)\) with the result \(y_2(t)\), then if the combined signal of \(x_1(t)\) and \(x_2(t)\) is input into the system, the result will be the combination of \(y_1(t)\) and \(y_2(t)\). The following diagram makes it easier to understand.

![Additivity](https://i.imgur.com/7LqaYR2.png)

**Superposition**

This term also encompasses the concept of linearity. What does this mean? It combines the properties of scaling and additivity. When signals are individually scaled and added, the resulting output is also scaled and combined in the same manner. The following diagram makes it easier to understand.

![Superposition](https://i.imgur.com/ynpN1Qi.png)

Next, let's look at time invariance.

### Time Invariant

This concept is easier to understand if you think of it as a translation in mathematics. The following diagram makes it clearer.

![Time Invariant](https://i.imgur.com/9X7aSHX.png)

### Why Use an LTI System?

LTI systems are advantageous because they are predictable. We will discuss the details of this advantage in future sections.

# Korean

## LTI 시스템

LTI는 Linear Time Invariant의 약자이다.

이를 하나하나 분석해볼 것이다.

### 선형성(Linear)

이 단어 또한 두 가지로 생각할 수 있다. 첫 번째 경우를 보자.

**스케일링과 가법성(Scaling + Additivity)**

먼저, 스케일링이란 무엇인가? 이는 입력 신호 함수에 상수를 곱했을 때, 출력 신호 함수의 결과도 상수를 곱한 것과 동일한 결과를 내는 성질이다. 다음 그림을 보면 이해가 쉬울 것이다.

![Scaling](https://i.imgur.com/W1x0SzN.png)

다음으로 가법성을 보자. 이는 입력 신호가 \(x_1(t)\)일 때 결과가 \(y_1(t)\)이고, 입력 신호가 \(x_2(t)\)일 때 결과가 \(y_2(t)\)일 때, \(x_1(t)\)신호와 \(x_2(t)\) 신호를 더한 신호를 시스템에 입력했을 경우, 결과 값이 \(y_1(t)\)와 \(y_2(t)\)를 더한 결과가 나오는 성질이다. 다음 그림을 보면 이해가 쉬울 것이다.

![Additivity](https://i.imgur.com/7LqaYR2.png)

**중첩의 원리(Superposition)**

이 단어로도 선형성을 생각할 수 있다. 이는 무슨 의미일까? 위의 스케일링과 가법성을 합한 것이라고 생각하면 된다. 각각의 신호에 상수를 곱하고 더한 경우, 해당 결과가 상수 배하고, 결과가 동일하다는 것이다. 다음 그림을 보면 이해에 도움이 될 것이다.

![Superposition](https://i.imgur.com/ynpN1Qi.png)

다음으로 시간 불변성을 살펴보자.

### 시간 불변성(Time Invariant)

이 경우는 수학에서 평행 이동을 생각하면 쉽다. 다음 그림을 보면 이해가 쉬울 것이다.

![Time Invariant](https://i.imgur.com/9X7aSHX.png)

### LTI 시스템을 사용하는 이유는 무엇일까?

LTI 시스템은 예측이 가능하다는 점에서 매우 유리한 시스템이다. 이에 대한 자세한 얘기는 추후에 다뤄볼 것이다.
