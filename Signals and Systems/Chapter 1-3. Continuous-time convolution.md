# English

### Continuous-Time Convolution

In the previous chapter, we discussed discrete-time convolution. However, in the real world, discrete time doesn’t actually exist. Therefore, let's explore how continuous-time convolution works.

Take a look at the following graph:

![conti](https://i.imgur.com/XLfmGcb.png)

Consider a signal like the one above. If we break down each part of the signal into rectangles, the graph would look like this:

![cont2](https://i.imgur.com/1r5xnwL.png)

Let’s denote the interval as $\Delta$. The area of the first rectangle can be calculated as follows:

$$
S_1 = x(0) \times \delta_{\Delta}(t) \times \Delta
$$

Similarly, the area of the second rectangle can be calculated as:

$$
S_2 = x(\Delta) \times \delta_{\Delta}(t- \Delta) \times \Delta
$$

You can continue to use this method for subsequent rectangles. As in discrete time, we can express this using a summation:

$$
x(t) = \lim_{\Delta → 0} \sum_{k = - \infty} ^{\infty} x (k \Delta) \delta_{\Delta}(t-k \Delta) \Delta
$$

This equation suggests that we can express it in the form of an integral, which students familiar with Riemann sums might recognize. However, note that this equation uses a unique variable like $k \Delta$. From now on, we will consider this variable as $\tau$. Reflecting this in a Riemann sum format gives us:

$$
x(t) = \int_{-\infty}^{\infty} x(\tau) h(t - \tau) d \tau
$$

Thus, we can finally understand the equation mentioned in Chapter 1-2:

$$
y(t) = f(x(t), ~h(t)) = x(t) * h(t)
$$

The above equation can be interpreted in various ways. Up until now, we have analyzed it in the $t$-domain. However, to solve problems or analyze situations, we must also be able to interpret it in the $\tau$-domain.

$$
x(t) = \int_{-\infty}^{\infty} x(\tau) h(t - \tau) d \tau
$$

The steps to interpret the equation are as follows:

1. Interpret $x(t)$ as $x(\tau)$.
2. Interpret $h(t)$ as $h(\tau)$.
3. Interpret $h(\tau)$ as $h(-\tau)$.
4. Interpret $h(-(\tau - t))$ as $h(t - \tau)$.

The following diagram illustrates this concept:

![conti4](https://i.imgur.com/vX6BryU.png)

The circled $t$ can be thought of as a dynamic value.

Now, since $x(\tau)$ and $h(t - \tau)$ are multiplied, consider their interaction as follows:

![conti5](https://i.imgur.com/P1yfNDA.png)

The result of this interaction can be expressed as:

$$
y(t) = \begin{cases}
t + 2 &t > -2 \\
2 & t = 0 \\
2-t & t < 2
\end{cases}
$$

The resulting graph is shown below:

![conti6](https://i.imgur.com/AJpmlDO.png)

Understanding this concept will be beneficial as you move forward.


# korean

### 연속시간 컨벌루션

이전 챕터에서, 이산 시간에 대한 내용을 다루었다. 하지만 우리가 살고 있는 세상은 이산적인 시간이란 사실상 존재할 수 없다. 그렇기에 연속시간 컨벌루션은 어떻게 생각할 수 있는지 알아보자.

아래의 그래프를 보자:

![conti](https://i.imgur.com/XLfmGcb.png)

다음과 같이 진행되는 신호에서 각 부분을 사각형으로 나누어 생각해보면 그림은 아래와 같다:

![cont2](https://i.imgur.com/1r5xnwL.png)

간격을 $\Delta$라 하고, 가장 첫 번째 사각형의 넓이를 구하면 다음과 같다:

$$
S_1 = x(0) \times \delta_{\Delta}(t) \times \Delta
$$

이와 같은 방법으로, 두 번째 사각형의 넓이를 구하면 다음과 같다:

$$
S_2 = x(\Delta) \times \delta_{\Delta}(t- \Delta) \times \Delta
$$

계속해서 같은 방법을 사용할 수 있을 것이다. 이를 이산 시간에서와 마찬가지로 시그마를 이용해서 표현하면 다음과 같을 것이다:

$$
x(t) = \lim_{\Delta → 0} \sum_{k = - \infty} ^{\infty} x (k \Delta) \delta_{\Delta}(t-k \Delta) \Delta
$$

위의 식만 보면 적분의 형태로 표현할 수 있을 것 같다는 생각이 들 것이다. 리만 합을 배운 학생들이라면 그렇다. 하지만, 식의 꼴을 보면 $k \Delta$와 같은 특이한 변수로 표현되어 있음을 알 수 있다. 이를 우리는 이제부터 $\tau$라는 변수로 생각할 것이다. 이를 반영해서 리만 합으로 표현하면 다음과 같을 것이다:

$$
x(t) = \int_{-\infty}^{\infty} x(\tau) h(t - \tau) d \tau
$$

즉, 최종적으로 챕터 1-2에서 언급한 다음과 같은 수식을 이해할 수 있다:

$$
y(t) = f(x(t), ~h(t) ) = x(t) * h(t)
$$

위의 식은 나타낼 수 있는 여러 가지 표현임을 알고 넘어가자. 지금까지 우리는 $t$-도메인으로 해석을 했다. 하지만, 우리는 문제를 풀거나 상황을 해석하기 위해 $t$ 말고도 $\tau$-도메인으로 해석할 줄 알아야 한다.

$$
x(t) = \int_{-\infty}^{\infty} x(\tau) h(t - \tau) d \tau
$$

위의 식을 해석하는 방법은 다음과 같다:

1. $x(t)$ → $x(\tau)$로 해석
2. $h(t)$ → $h(\tau)$로 해석
3. $h(\tau)$ → $h(-\tau)$로 해석
4. $h(-(\tau - t)) = h(t - \tau)$

즉, 아래의 그림과 같이 생각하면 쉬울 것이다:

![conti4](https://i.imgur.com/vX6BryU.png)

동그라미 친 $t$는 유동적인 값이라 생각하면 된다.

정지한 $x(\tau)$와 $h(t - \tau)$가 곱해진 꼴이므로 관통한다고 생각하면 다음과 같을 것이다:

![conti5](https://i.imgur.com/P1yfNDA.png)

이때, 결과를 살펴보면 다음과 같다:

$$
y(t) = \begin{cases}
t + 2 &t > -2 \\
2 & t = 0 \\
2-t & t < 2
\end{cases}
$$

이 결과를 그래프로 나타내면 다음과 같다:

![conti6](https://i.imgur.com/AJpmlDO.png)

이런 내용을 잘 알고 넘어가면 좋을 것 같다.




