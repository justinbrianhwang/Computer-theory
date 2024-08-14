# English


### Linear constant-coefficient differential equation

A linear constant-coefficient differential equation is a differential equation where the coefficients of $x$ or $y$ are constants that do not change. It can be expressed mathematically as follows:

$$
\sum_{k=0}^{N} a_k \frac{d^k y(t)}{dt^k} = \sum_{k=0}^{N} b_k \frac{d^k x(t)}{dt^k}
$$

So far, we have looked at simpler forms of equations.

![linear](https://i.imgur.com/bi9MQDx.png)

This is a simple first-order equation. However, real-world systems are often modeled by differential equations of this form. To better understand this, we will explore two examples.

First, let's consider a physical example.

Take a look at the following diagram:

![car](https://i.imgur.com/rAFWRjL.png)

Let's calculate the net acceleration of the car. To find the net acceleration, we first need to determine the net force, which is the driving force minus the frictional force. The net acceleration can then be calculated as follows:

$$
F = ma
$$

$$
f(t)-\rho v(t) = ma
$$

$$
a = \frac{f(t)-\rho v(t)}{m}
$$

If we express $a$ in terms of velocity, we get:

$$
\frac{dv(t)}{dt} = \frac{f(t)-\rho v(t)}{m}
$$

This equation can be separated into input and output terms:

$$
\frac{dv(t)}{dt} + \frac{\rho}{m} v(t) = \frac{f(t)}{m}
$$

Here, the input is $f(t)$, and the output is $v(t)$. This is an example of an LCCDE.

Next, let's consider an electrical circuit.

Take a look at the following circuit diagram:

![circuit](https://i.imgur.com/m5qgsn3.png)

Using Ohm's law, we can find the net voltage $V_s - V_c$ and calculate the current as follows:

$$
l(t) = \frac{V_s(t) - V_c(t)}{R} = C \frac{dV_c(t)}{dt}
$$

Similarly, we can separate the input and output terms:

$$
\frac{dV_c(t)}{dt} + \frac{1}{RC} V_c(t) = \frac{1}{RC} V_s(t)
$$

In this case, the input is $V_s(t)$, and the output is $V_c(t)$. Differential equations like this will be encountered frequently in system analysis.

For more detailed explanations on solving differential equations, please refer to the following directory:

[differential equation](https://github.com/justinbrianhwang/Mathematics/tree/main/Engineering%20mathematics)



# Korean

### Linear constant-coefficient differential equation

$x$ 또는 $y$의 계수가 변하지 않는 상수로 이루어진 미분 방정식을 뜻한다. 즉, 식으로 표현하면 아래와 같다.

$$
\sum_{k=0}^{N} a_k \frac{d^k y(t)}{dt^k} = \sum_{k=0}^{N} b_k \frac{d^k x(t)}{dt^k}
$$

지금까지는 단순한 형태를 보았다.

![linear](https://i.imgur.com/bi9MQDx.png)

위와 같이 단순하게 1차 방정식과 같은 형태이다. 하지만, 실제 시스템은 주로 미분 방정식과 같은 형태로 나타난다. 이를 명확히 이해하기 위해 두 가지 예시를 살펴볼 것이다.

먼저, 물리학적인 예시를 보자.

다음 그림을 살펴보자.

![car](https://i.imgur.com/rAFWRjL.png)

이 차의 알짜 가속도를 구해보자. 먼저, 알짜 가속도를 구하기 위해서는 알짜 힘을 구해야 하는데, 알짜 힘은 추진력에서 마찰력을 뺀 것이다. 이를 적용하여 알짜 가속도를 구하면 다음과 같다:

$$
F = ma
$$

$$
f(t)-\rho v(t) = ma
$$

$$
a = \frac{f(t)-\rho v(t)}{m}
$$

이때 $a$를 속도로 표현하면 다음과 같다:

$$
\frac{dv(t)}{dt} = \frac{f(t)-\rho v(t)}{m}
$$

위의 식을 입력과 출력으로 나누면 된다:

$$
\frac{dv(t)}{dt} + \frac{\rho}{m} v(t) = \frac{f(t)}{m}
$$

이와 같이 식이 정리된다. 이때 입력은 $f(t)$이고, 출력은 $v(t)$이다. 이러한 상황을 우리가 LCCDE라고 한다.

이와 유사한 상황으로 회로의 예를 보자.

다음과 같은 회로도를 보자.

![circuit](https://i.imgur.com/m5qgsn3.png)

이때 전류를 옴의 법칙을 이용하여 알짜 전력인 $V_s - V_c$를 구하면 아래와 같다:

$$
l(t) = \frac{V_s(t) - V_c(t)}{R} = C \frac{dV_c(t)}{dt}
$$

마찬가지로, 이 식을 입력과 출력을 구분하기 위해 정리하면 다음과 같다:

$$
\frac{dV_c(t)}{dt} + \frac{1}{RC} V_c(t) = \frac{1}{RC} V_s(t)
$$

이와 같이 입력은 $V_s(t)$이고, 출력은 $V_c(t)$이다. 이러한 미분 방정식 상황은 앞으로 많이 다루게 될 것이다.

미분 방정식의 풀이에 대해서는 다음 디렉터리에서 자세히 설명해 놓았다. 이를 참고하여 앞으로의 공부에 도움이 되기를 바란다.

[differential equation](https://github.com/justinbrianhwang/Mathematics/tree/main/Engineering%20mathematics)








