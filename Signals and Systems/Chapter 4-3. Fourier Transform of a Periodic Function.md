
# Fourier Transform of a Periodic Function

**Problem:** Find the Fourier transform of $\cos(\omega_0 t)$.

At first glance, this might seem strange. The purpose of the **Fourier Transform** is to represent **aperiodic signals** in a manner similar to the Fourier series. However, here we are asked to find the transform of a typical **periodic function**, $\cos(\omega_0 t)$.

This might seem like an odd example, but let’s look at the following diagram:

![cos](https://i.imgur.com/3xGX6QN.png)

Is the function above periodic?

If we only consider the visible part, it appears to be periodic. But what if the graph changes form at some arbitrary point $T_0$?

![cos2](https://i.imgur.com/VSVtNS9.png)

Is this function still periodic? Clearly, **it is not**. However, if we let $T_0 \to \infty$, the function would appear periodic again.

This is an extreme example, but it shows that while the primary purpose of the Fourier Transform is to handle **aperiodic signals**, there’s no issue in applying it to periodic functions as well.

Additionally, the function $\cos(\omega_0 t)$ does not satisfy the **absolute integrability condition**. Most periodic functions fail to meet the **Dirichlet conditions**. However, they can still be transformed using the Fourier Transform.

Let’s proceed with finding the Fourier Transform of $\cos(\omega_0 t)$:

$$
\int_{-\infty}^{\infty} \cos(\omega_0 t) e^{-j\omega t} \, dt
$$

This integral is challenging to solve directly, so let’s use the **complex exponential representation**:

$$
\cos(\omega t) = \frac{e^{j\omega t} + e^{-j\omega t}}{2}
$$

We need to find the transform of $e^{j\omega t}$ first:

$$
e^{j\omega t} = \frac{1}{2\pi} \int_{-\infty}^{\infty} \Box \, e^{j\omega_0 t} \, d\omega_0
$$

Now, let’s deduce what belongs in the box (▭).

**Result of deduction:**

$$
\Box = 2\pi\delta(\omega - \omega_0)
$$

Substituting this back, we find that the expression holds true. This approach uses **one-to-one correspondence**, and while it might seem like a guess, there is no mathematical error in this deduction.

Thus, the Fourier Transform of $\cos(\omega_0 t)$ is:

$$
\int_{-\infty}^{\infty} \cos(\omega_0 t) e^{-j\omega t} \, dt = \pi\left[\delta(\omega - \omega_0) + \delta(\omega + \omega_0)\right]
$$

Through this process, we see that **periodic functions can also be transformed** using the Fourier Transform. Make sure to study the **Fourier Transform table** from the previous chapter for useful reference.


# 주기 함수의 푸리에 변환

**문제:** $\cos(\omega_0 t)$의 푸리에 변환을 구하라.

위의 질문을 보면 이상함을 느껴야 한다. 우리가 **푸리에 변환**을 하는 이유는 **비주기 신호**를 푸리에 급수처럼 표현하기 위함이었다. 그런데 대표적인 **주기 함수**인 $\cos(\omega_0 t)$를 푸리에 변환하라는 문제는 다소 이상해 보인다.

이상한 예시일 수 있지만, 다음 그림을 보자.

![cos](https://i.imgur.com/3xGX6QN.png)

위의 함수는 주기 함수일까?

위의 부분만 보면 맞는 것 같지만, 극단적으로 임의의 점 $T_0$부터 형태가 바뀌는 그래프를 생각해보자.

![cos2](https://i.imgur.com/VSVtNS9.png)

이 함수는 주기 함수일까? 당연히 **주기 함수는 아니다**. 하지만 $T_0 \to \infty$로 보내면, 이는 다시 주기 함수가 된다.

물론, 이 예시는 극단적인 경우이지만, 원래는 **비주기 함수를 푸리에 변환**하는 것이 목적이다. 그러나 **주기 함수도 푸리에 변환**을 할 수 있다는 점을 기억하자.

또한, $\cos(\omega_0 t)$는 **절대 적분 가능 조건**을 만족시키지 않는다. 즉, 대부분의 **주기 함수는 디리클레 조건**을 만족시키지 않는다. 하지만 이 함수들도 푸리에 변환이 가능하다!

이제 $\cos(\omega_0 t)$의 푸리에 변환을 구해보자.

$$
\int_{-\infty}^{\infty} \cos(\omega_0 t) e^{-j\omega t} \, dt
$$

위의 계산을 직접 수행할 수도 있지만, 다소 복잡하므로 **복소 지수함수 표현**을 이용하자.

$\cos(\omega_0 t)$를 복소 지수함수로 나타내면:

$$
\cos(\omega t) = \frac{e^{j\omega t} + e^{-j\omega t}}{2}
$$

이제 부호만 반대인 $e^{j\omega t}$의 푸리에 변환을 구해보자.

$$
e^{j\omega t} = \frac{1}{2\pi} \int_{-\infty}^{\infty} \Box \, e^{j\omega_0 t} \, d\omega_0
$$

여기서, 네모칸(▭) 안의 표현을 추론해야 한다.

**추론 결과:**

$$
\Box = 2\pi\delta(\omega - \omega_0)
$$

실제로 위의 표현을 대입해보면, **일대일 대응** 관계를 이용하여 성립함을 알 수 있다. 약간은 직관적으로 추론했지만, 수학적 오류는 없으므로 받아들일 수 있다.

따라서, $\cos(\omega_0 t)$의 푸리에 변환은 다음과 같다:

$$
\int_{-\infty}^{\infty} \cos(\omega_0 t) e^{-j\omega t} \, dt = \pi\left[\delta(\omega - \omega_0) + \delta(\omega + \omega_0)\right]
$$

이 과정을 통해 **주기 함수도 푸리에 변환을 구할 수 있음**을 이해하고 넘어가자. 이전 장에서 제시한 **푸리에 변환 테이블**을 잘 암기하고 활용하면 도움이 될 것이다.
