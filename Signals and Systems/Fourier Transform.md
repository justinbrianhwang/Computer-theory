
## Fourier Transform

The **Fourier Transform** can be viewed as an extension of the **Fourier series**.

The Fourier series decomposes **periodic signals** into basic sinusoidal components. However, we need to extend this analysis to **aperiodic signals**.

Let’s consider the following scenario:

![ss](https://i.imgur.com/mMrnymb.png)

The image above shows a signal with a period of $4$. We can easily see that this signal has a period of $4$. Now, let’s generalize this to a signal with a period of $T_0$:

![ss](https://i.imgur.com/dVu2BTk.png)

The image represents a signal with a period of $T_0$. What happens if we let $T_0 \to \infty$?

It would appear as if there is only one rectangular pulse centered at $0$.

Thus, we interpret **aperiodic signals** as signals with an **infinite period**.

Now, let’s examine the formula for the Fourier series coefficients.

### Deriving the Fourier Transform from Fourier Series Coefficients

The formula for the Fourier series coefficients is:

$$
a_k = \frac{1}{T_0} \int_{-\frac{1}{T_0}}^{\frac{1}{T_0}} x_{T_0}(t) e^{-jk\omega_0 t} \, dt
$$

Multiplying both sides by $T_0$ gives:

$$
a_k T_0 = \int_{-\frac{1}{T_0}}^{\frac{1}{T_0}} x_{T_0}(t) e^{-jk\omega_0 t} \, dt
$$

Now, assuming we are dealing with an **aperiodic signal**, let $T_0 \to \infty$:

$$
\lim_{T_0 \to \infty} a_k T_0 = \lim_{T_0 \to \infty} \int_{-\frac{1}{T_0}}^{\frac{1}{T_0}} x_{T_0}(t) e^{-jk\omega_0 t} \, dt
$$

We will simplify the notation by making the following substitutions:

- As $T_0 \to \infty$:
- $x_{T_0}(t) \to x(t)$
- $a_k T_0 \triangleq X(k\omega_0)$
- $k\omega_0 \triangleq \omega$

Thus, we can express the equation as:

$$
X(\omega) = \int_{-\infty}^{\infty} x(t) e^{-j\omega t} \, dt
$$

This is the **Fourier Transform** formula. What about the **inverse transform**?

The inverse formula is derived from the Fourier series using a similar process. We won’t prove it here, but the formula is:

$$
x(t) = \frac{1}{2\pi} \int_{-\infty}^{\infty} X(\omega) e^{j\omega t} \, d\omega
$$

Understand that this formula is derived from the Fourier series.

In the next chapter, we will interpret the Fourier Transform.

## 푸리에 변환

우리가 기존에 배웠던 **푸리에 급수**의 확장판이라 생각하면 이해가 쉽다.

푸리에 급수는 **주기 신호**를 우리가 알고 있는 기본 신호들로 표현하는 것이다. 이번에는 **비주기 신호**를 확장하여 분석할 것이다.

먼저 다음과 같은 상황을 떠올려보자.

![ss](https://i.imgur.com/mMrnymb.png)

위의 그림은 주기가 $4$인 신호를 나타낸 것이다. 이런 신호는 직관적으로 주기가 $4$임을 알 수 있다. 이제 이 신호를 일반화하여 다음과 같이 나타내보자.

![ss](https://i.imgur.com/dVu2BTk.png)

위의 그림은 주기가 $T_0$인 신호를 나타낸 것이다. 이제, 주기 $T_0$을 $T_0 \to \infty$로 보내면 어떻게 될까?

이는 0에서만 사각 펄스가 하나 있는 것처럼 보인다.

즉, **비주기 신호**는 **주기가 무한인 신호**로 해석할 수 있는 것이다.

이제 푸리에 급수의 계수 정의식을 살펴보자.

### 푸리에 급수 계수로부터 유도한 푸리에 변환

푸리에 급수의 계수는 다음과 같다:

$$
a_k = \frac{1}{T_0} \int_{-\frac{1}{T_0}}^{\frac{1}{T_0}} x_{T_0}(t) e^{-jk\omega_0 t} \, dt
$$

여기서 양변에 $T_0$을 곱하면:

$$
a_k T_0 = \int_{-\frac{1}{T_0}}^{\frac{1}{T_0}} x_{T_0}(t) e^{-jk\omega_0 t} \, dt
$$

이제 우리는 **비주기 신호**를 가정하고, $T_0 \to \infty$로 생각해보자.

$$
\lim_{T_0 \to \infty} a_k T_0 = \lim_{T_0 \to \infty} \int_{-\frac{1}{T_0}}^{\frac{1}{T_0}} x_{T_0}(t) e^{-jk\omega_0 t} \, dt
$$

이제 치환을 통해 표현을 간단하게 만들 것이다:

- $T_0 \to \infty$일 때:
- $x_{T_0}(t) \to x(t)$
- $a_k T_0 \triangleq X(k\omega_0)$
- $k\omega_0 \triangleq \omega$

따라서, 위의 식은 다음과 같이 표현된다:

$$
X(\omega) = \int_{-\infty}^{\infty} x(t) e^{-j\omega t} \, dt
$$

이 식이 바로 **푸리에 변환식**이다. 그렇다면 **역변환식**은 어떻게 될까?

역변환식은 푸리에 급수식으로부터 유도되며, 비슷한 과정을 통해 얻어진다. 여기서는 증명은 생략하고, 식만 제시하겠다:

$$
x(t) = \frac{1}{2\pi} \int_{-\infty}^{\infty} X(\omega) e^{j\omega t} \, d\omega
$$

결국 푸리에 급수 식으로부터 유도되었음을 이해하고 넘어가도록 하자.

다음 장에서는 푸리에 변환에 대한 해석을 다룰 것이다.

