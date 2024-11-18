# Fourier Transform of Unit Step Function

We previously skipped proving the Fourier transforms of most functions, including the unit step function. However, we will prove the Fourier transform of the **unit step function** here, as its form is quite unique. This process helps build a foundation for approaching similar problems in the future.

### Problem Setup

Consider the function formed by multiplying the unit step function $u(t)$ with an exponential function $e^{-at}$:

$$
\lim_{a \to 0} e^{-at} u(t)
$$

The Fourier transform of this function is:

$$
\lim_{a \to 0} \int_{0}^{\infty} e^{-at} e^{-j\omega t} \, dt = \lim_{a \to 0} \frac{e^{-at - j\omega t} \Big|_{0}^{\infty}}{-a - j\omega} = \lim_{a \to 0} \frac{1}{a + j\omega}
$$

It might seem like we can directly substitute $a \to 0$, but we cannot due to the properties of limits.

### Properties of Limits

When $\omega = 0$, the expression simplifies to $\frac{1}{a}$. The following diagram helps illustrate the limits:

![aa](https://i.imgur.com/AthWEwk.png)

- Left-hand limit: $-\infty$
- Right-hand limit: $\infty$

Since the limit does not exist, we cannot directly substitute $a \to 0$.

### Realization Process

Multiply both numerator and denominator by $a - j\omega$:

$$
\lim_{a \to 0} \frac{1}{a + j\omega} \times \frac{a - j\omega}{a - j\omega} = \lim_{a \to 0} \left(\frac{a}{a^2 + \omega^2} - \frac{j\omega}{a^2 + \omega^2}\right)
$$

Let $\frac{a}{a^2 + \omega^2}$ be $f(\omega)$ and take the limit as $a \to 0$:

$$
\lim_{a \to 0} \left(f(\omega) + \frac{1}{j\omega}\right)
$$

Thus, the Fourier transform of the unit step function $u(t)$ is:

$$
\mathcal{F}\left(u(t)\right) = \pi \delta(\omega) + \frac{1}{j\omega}
$$

### Fourier Transform of $u(t) + u(-t)$

Now consider the Fourier transform of $u(t) + u(-t)$, which is always equal to $1$. The transform of $1$ is:

$$
1 \quad \xleftrightarrow{\mathcal{F}} \quad 2\pi \delta(\omega)
$$

Verification through calculation:

$$
u(t) \quad \xleftrightarrow{\mathcal{F}} \quad f(\omega) + \frac{1}{j\omega}
$$

$$
u(-t) \quad \xleftrightarrow{\mathcal{F}} \quad f(-\omega) - \frac{1}{j\omega}
$$

Adding the two gives:

$$
u(t) + u(-t) \quad \xleftrightarrow{\mathcal{F}} \quad f(-\omega) + f(\omega)
$$

Thus:

$$
1 \quad \xleftrightarrow{\mathcal{F}} \quad 2f(\omega)
$$

We find:

$$
f(\omega) = \pi \delta(\omega)
$$

Therefore, the Fourier transform of the unit step function is:

$$
\mathcal{F}\left(u(t)\right) = \pi \delta(\omega) + \frac{1}{j\omega}
$$

### Conclusion

We have proved the Fourier transform of the unit step function $u(t)$. Following this process helps deepen the understanding of integral transforms.


# 단위 계단 함수의 푸리에 변환

단위 계단 함수를 포함한 대부분의 푸리에 변환은 이전에 증명을 생략했지만, 단위 계단 함수의 푸리에 변환은 복잡하고 특이한 형태를 가지기 때문에 이 증명을 진행한다. 이를 통해 비슷한 문제에서도 빠르게 접근할 수 있는 기반을 마련할 수 있다.

### 문제 설정

단위 계단 함수 $u(t)$에 지수 함수 $e^{-at}$를 곱한 꼴의 함수를 생각해보자:

$$
\lim_{a \to 0} e^{-at} u(t)
$$

이 함수를 푸리에 변환하면 다음과 같은 식이 된다. (일부 수식적 생략 포함)

$$
\lim_{a \to 0} \int_{0}^{\infty} e^{-at} e^{-j\omega t} \, dt = \lim_{a \to 0} \frac{e^{-at - j\omega t} \Big|_{0}^{\infty}}{-a - j\omega} = \lim_{a \to 0} \frac{1}{a + j\omega}
$$

이 식을 보면, $a \to 0$을 바로 대입하면 될 것 같지만, 바로 대입할 수 없다. 이는 극한의 성질과 관련이 있다.

### 극한의 성질

$\omega = 0$인 경우, 함수의 꼴은 $\frac{1}{a}$가 된다. 아래 그림을 보면 극한을 직관적으로 이해할 수 있다:

![aa](https://i.imgur.com/AthWEwk.png)

- 좌극한: $-\infty$
- 우극한: $\infty$

따라서 극한 값이 존재하지 않으므로, $a \to 0$으로 극한을 바로 취할 수 없다.

### 실수화 과정

이제 분모와 분자에 $a - j\omega$를 곱해보자:

$$
\lim_{a \to 0} \frac{1}{a + j\omega} \times \frac{a - j\omega}{a - j\omega} = \lim_{a \to 0} \left(\frac{a}{a^2 + \omega^2} - \frac{j\omega}{a^2 + \omega^2}\right)
$$

이제 $\frac{a}{a^2 + \omega^2}$를 $f(\omega)$라 두고, $a \to 0$을 보내면:

$$
\lim_{a \to 0} \left(f(\omega) + \frac{1}{j\omega}\right)
$$

결국 $a = 0$일 때, 단위 계단 함수 $u(t)$의 푸리에 변환은 다음과 같다:

$$
\mathcal{F}\left(u(t)\right) = \pi \delta(\omega) + \frac{1}{j\omega}
$$

### $u(t)$와 $u(-t)$의 합의 푸리에 변환

이제 $u(t) + u(-t)$의 푸리에 변환을 구해보자. $u(t) + u(-t)$는 항상 $1$이므로, $1$의 푸리에 변환은 다음과 같이 나타난다:

$$
1 \quad \xleftrightarrow{\mathcal{F}} \quad 2\pi \delta(\omega)
$$

이를 계산 과정을 통해 확인해보자:

$$
u(t) \quad \xleftrightarrow{\mathcal{F}} \quad f(\omega) + \frac{1}{j\omega}
$$

$$
u(-t) \quad \xleftrightarrow{\mathcal{F}} \quad f(-\omega) - \frac{1}{j\omega}
$$

두 식을 더하면:

$$
u(t) + u(-t) \quad \xleftrightarrow{\mathcal{F}} \quad f(-\omega) + f(\omega) - \frac{1}{j\omega} + \frac{1}{j\omega}
$$

이제 $f(\omega) = f(-\omega)$라는 성질을 이용하면:

$$
1 \quad \xleftrightarrow{\mathcal{F}} \quad 2f(\omega)
$$

따라서:

$$
2f(\omega) = 2\pi \delta(\omega)
$$

이를 통해 $f(\omega) = \pi \delta(\omega)$임을 알 수 있고, 단위 계단 함수의 푸리에 변환은:

$$
\mathcal{F}\left(u(t)\right) = \pi \delta(\omega) + \frac{1}{j\omega}
$$

### 결론

단위 계단 함수 $u(t)$의 푸리에 변환을 증명했다. 이 과정을 직접 따라 해보는 것은 적분 변환의 이해를 돕는 데 큰 도움이 될 것이다.
