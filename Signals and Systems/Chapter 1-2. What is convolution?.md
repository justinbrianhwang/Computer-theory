# English

## Impulse Function

$$
y = f(x(t), ~h(t))
$$

What is $h(t)$ in the above equation?

$h(t)$ is called the impulse response. To understand the impulse response, we first need to understand the impulse function, which is usually denoted as $\delta[n]$. The graphical representation of this function is shown below.

![impulse function](https://i.imgur.com/bopGSGd.png)

Mathematically, this function can be defined as:

$$
\delta[n] = \begin{cases}
1 & n = 0 \\
0 & n \neq 0
\end{cases}
$$

This function satisfies the following properties:

$$
\begin{cases}
\sum_{n=-\infty}^{\infty} \delta[n] = 1 \\
\sum_{n=-\infty}^{\infty} f[n] \delta[n] = f[0]
\end{cases}
$$

A function satisfying these properties is known as an impulse function.

Let's consider an example where the area under a given function is 1. It is clear that $\lim_{\Delta → 0} \delta_{\Delta}(t)$ yields a value of 1 at $t = 0$. Therefore, $\lim_{\Delta → 0} \delta_{\Delta}(t)$ can be considered as $\delta[n]$.

### Definition of Function $h(t)$

Now that we have defined the impulse function, let’s consider the process of applying this function to an LTI system. This process is illustrated in the following diagram.

![LTI system](https://i.imgur.com/bCfNH2o.png)

In this diagram, $h(t)$ represents the impulse response. But why do we use the impulse response?

Consider the design of an opera house, where the walls are shaped in a particular way to minimize sound differences across various seats. In any standard room, such as a classroom or a home, the wall shapes differ significantly from those found in an opera hall.

![opera hall](https://i.imgur.com/5AOy0z5.png)

In opera halls, the unique wall shapes help ensure that the sound is evenly distributed across all seating areas. Sound is a type of wave, which diminishes with distance, causing differences in how it is perceived in different seats. Some areas might experience constructive or destructive interference, leading to amplified or reduced sound. The design of these walls helps mitigate such issues.

From now on, we will use $\delta(t)$ to refer to the impulse function and $h(t)$ to refer to the impulse response.

Returning to our initial equation:

$$
y(t) = f(x(t), ~ h(t))
$$

What does the function $f$ represent? This function is known as convolution. Convolution can be understood as the process of calculating cumulative responses. To explain this concept, consider the example of pressing a pillow.

Assume the pillow is made of latex. When pressure is applied and released, the pillow takes time to return to its original shape. Let's denote the applied force as $F$.

![con](https://i.imgur.com/vu20OH5.png)

Now, if the pillow is pressed with twice the force, $2F$, the response will be twice as strong.

![con2](https://i.imgur.com/ZVcgR67.png)

What happens if we press the pillow three times at regular intervals? The resulting graph will look like this:

![com3](https://i.imgur.com/AQS1tSu.png)

The final response is simply the sum of the individual responses. Convolution is essentially this concept, where the response to a signal is the sum of the responses to individual impulses. In this context, pressing the pillow can be thought of as applying an impulse.

### Combining Signals

Signals can be represented as the sum of impulses. Let’s consider a discrete-time scenario with the function $x[n]$, as shown below.

![am](https://i.imgur.com/qCHB8sS.png)

This function can be represented as a sum of impulses, similar to how a Taylor series represents a function as the sum of polynomial terms. For example, the function $f(x)$ can be expressed as:

$$
f(x) = c_0 + c_1 x + c_2 x^2 + \cdots
$$

Similarly, $x[n]$ can be expressed as a sum of shifted and scaled impulses. Assume $x[n]$ has values of 3 at $n = 0$, 2 at $n = 1$, and 1 at $n = 2$. We can express $x[n]$ using the impulse function as follows:

$$
x[n] = \begin{cases}
n=0 & 3 \delta[n] \\
n=1 & 2 \delta[n-1] \\
n=2 & \delta[n-2]
\end{cases}
$$

Adding these values together gives us:

$$
x[n] = 3 \delta[n] + 2 \delta[n - 1] + \delta[n - 2]
$$

Since the system we are dealing with is an LTI system, it satisfies linearity, so adding these inputs will produce the corresponding output:

$$
y[n] = \begin{cases}
n=0 & 3 h[n] \\
n=1 & 2 h[n-1] \\
n=2 & h[n-2]
\end{cases}
$$

However, expressing each case separately is not efficient, so it is more appropriate to use the summation symbol:

$$
x[n] = \sum_{k = -\infty} ^{\infty } x[k] \delta[n-k] 
$$
$$
y[n] = \sum_{k = -\infty} ^{\infty } x[k] h[n-k]
$$

This method of expression is known as convolution.


# Korean

## 임펄스 함수

$$
y = f(x(t), ~h(t))
$$

위의 수식에서 $h(t)$는 무엇일까?

$h(t)$는 임펄스 응답(impulse response)이라 한다. 임펄스 응답을 이해하기 위해 먼저 임펄스 함수에 대해 알아보자. 이 함수는 주로 $\delta[n]$로 표현된다. 이 함수의 개형은 아래와 같다.

![impulse function](https://i.imgur.com/bopGSGd.png)

이 함수를 수식으로 표현하면 다음과 같다.

$$
\delta[n] = \begin{cases}
1 & n = 0 \\
0 & n \neq 0
\end{cases}
$$

이 함수는 다음과 같은 성질을 만족한다.

$$
\begin{cases}
\sum_{n=-\infty}^{\infty} \delta[n] = 1 \\
\sum_{n=-\infty}^{\infty} f[n] \delta[n] = f[0]
\end{cases}
$$

이러한 성질을 만족하면 이 함수는 임펄스 함수라고 할 수 있다.

하나의 예를 들어보자. 아래와 같은 함수가 주어졌다고 가정하자.

![impulse function2](https://i.imgur.com/HWUr3Aw.png)

위의 함수의 넓이를 구해보면 $1$임을 알 수 있다. $\lim_{\Delta → 0} \delta_{\Delta}(t)$를 계산하면 결국 $t = 0$에서 $1$을 가지므로 $\lim_{\Delta → 0} \delta_{\Delta}(t)$는 $\delta[n]$라고 할 수 있다.

### 함수 $h(t)$ 정의

위에서 임펄스 함수를 정의했으니, 이 함수를 LTI 시스템에 입력하는 과정을 보자. 다음의 그림과 같다.

![LTI system](https://i.imgur.com/bCfNH2o.png)

이 그림에서 $h(t)$가 바로 임펄스 응답이다. 그렇다면, 임펄스 응답을 사용하는 이유는 무엇일까?

하나의 상황을 생각해보자. 예술 공연장에 가보면, 벽의 모양이 매우 특이하다는 것을 확인할 수 있다. 일반적인 교실이나 집의 벽 모양과는 다르게, 아래의 그림과 같은 모양을 하고 있다.

![opera hall](https://i.imgur.com/5AOy0z5.png)

이처럼 오페라 홀의 벽이 다른 모습인 이유는, 각 자리별로 소리의 차이를 줄이기 위해서이다. 소리는 기본적으로 파동의 형태이며, 멀어질수록 감소하는 경향이 있고, 자리마다 소리의 크기가 다르게 느껴진다. 심지어 간섭 현상이 발생하여 특정 자리에서는 소리가 상쇄되어 작아지고, 다른 자리에서는 소리가 증폭되어 커지는 경우가 있다. 이런 문제를 해결하기 위해 벽의 모양이 다르게 설계된다.

앞으로 우리는 $\delta(t)$를 임펄스 함수라고 하고, $h(t)$를 임펄스 응답이라고 부를 것이다.

그렇다면 처음에 본 수식인 $y(t) = f(x(t), ~ h(t))$에서 $f$는 무엇일까?

우리는 이를 컨볼루션(convolution)이라고 부른다. 컨볼루션은 누적된 반응을 계산하는 개념으로 이해할 수 있다. 예를 들어, 베개를 누르는 상황을 생각해보자.

베개가 라텍스 재질로 되어있다고 가정하고, 처음 누르기 시작한 후 다시 원래 상태로 돌아올 때까지의 과정을 측정하면 아래 그림처럼 나타낼 수 있다. 이때 힘을 $F$라고 하자.

![con](https://i.imgur.com/vu20OH5.png)

이제, 같은 간격으로 세 번 눌렀다고 가정해보자. 결과 그래프는 다음과 같다.

![com3](https://i.imgur.com/AQS1tSu.png)

결과적으로 이러한 개념을 컨볼루션이라고 할 수 있다. 어렵게 생각할 필요 없이 신호의 합성으로 이해하면 된다. 위의 예시에서 손으로 누르는 것 자체가 임펄스로 이해할 수 있다.

### 신호들의 합성

신호들은 임펄스의 합으로 나타낼 수 있다. 예를 들어 이산 시간 상황에서 $x[n]$ 함수를 가정해보자.

![am](https://i.imgur.com/qCHB8sS.png)

이 함수는 각각의 값에 대해 임펄스 함수의 합으로 나타낼 수 있다. 마치 테일러 급수로 임의의 함수를 다항함수의 합으로 나타내는 것과 유사하다. 

예를 들어, $f(x)$를 다항함수의 합으로 나타내기 위해 테일러 급수를 사용하는 방식이 있다.

$$
f(x) = c_0 + c_1 x + c_2 x^2 + \cdots
$$

이와 마찬가지로 $x[n]$을 $\delta[n]$로 표현할 수 있다. $x[n]$을 가정하면, $n = 0$에서 $3$, $n =1$ 에서 $2$, $n = 2$에서 $1$을 가지는 형태이다. 이때 $\delta$를 평행이동과 상수배를 통해 합으로 표현할 수 있다.

$$
x[n] = 
\begin{cases}
n=0&3 \delta[n] \\
n=1&2 \delta[n-1] \\
n=2& \delta[n-2]
\end{cases}
$$

즉, 이 값들을 전부 더해서 $x[n]$을 표현하면 다음과 같다.

$$
x[n] = 3 \delta[n] +  2\delta[n - 1] + \delta[n - 2]
$$

우리가 다루는 시스템은 LTI 시스템이므로 Linear한 성질을 만족하므로 각각을 전부 더한 경우도 출력 결과가 잘 나올 것이다.

즉, $x[n]$을 시스템에 넣은 결과인 $y[n]$은 다음과 같이 표현할 수 있다.

$$
y[n] = 
\begin{cases}
n=0&3 h[n] \\
n=1&2 h[n-1] \\
n=2& h[n-2]
\end{cases}
$$

이와 같이 각 케이스 별로 표현하기엔 부적절하니, 시그마 기호를 사용해서 나타내는 것이 적절할 것이다.

$$
x[n] = \sum_{k = -\infty} ^{\infty } x[k] \delta[n-k]
$$
$$
y[n] = \sum_{k = -\infty} ^{\infty } x[k] h[n-k]
$$

우리가 이렇게 표현하는 방식이 바로 컨볼루션이다.





