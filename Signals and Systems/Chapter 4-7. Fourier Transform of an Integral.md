# Fourier Transform of an Integral

Consider the following integral:

$$
\int_{-\infty}^{t} x(\tau) \, d\tau = x(t) \otimes u(t) = \int_{-\infty}^{\infty} x(\tau) u(t-\tau) \, d\tau
$$

This expression represents the **convolution** of $x(t)$ and the unit step function $u(t)$. What would be the **Fourier Transform** of $x(t) \otimes u(t)$?

According to the **Convolution Theorem** in Fourier analysis, the Fourier Transform of the convolution is given by:

$$
X(\omega) \times U(\omega)
$$

Let’s use the previously derived **Fourier Transform** of the unit step function:

$$
U(\omega) = \pi \delta(\omega) + \frac{1}{j\omega}
$$

Thus, the product $X(\omega) \times U(\omega)$ can be expressed as:

$$
X(\omega) U(\omega) = \pi \delta(\omega) X(\omega) + \frac{1}{j\omega} X(\omega)
$$

In conclusion, the Fourier Transform of an integral can be represented as a multiplication operation, and it can be solved using the Fourier Transform of the **unit step function**. It is recommended to work out the rest of the calculations directly for better understanding.

# 적분의 푸리에 변환

다음과 같은 적분 상황을 생각해보자:

$$
\int_{-\infty}^{t} x(\tau) \, d\tau = x(t) \otimes u(t) = \int_{-\infty}^{\infty} x(\tau) u(t-\tau) \, d\tau
$$

이 식은 $x(t)$와 단위 계단 함수 $u(t)$의 **컨볼루션**으로 나타낼 수 있다. 그렇다면 $x(t) \otimes u(t)$의 **푸리에 변환**은 어떻게 될까?

푸리에 변환의 **컨볼루션 정리**에 따르면, 이 식의 푸리에 변환은 다음과 같이 **곱셈**으로 표현할 수 있다:

$$
X(\omega) \times U(\omega)
$$

이제, 우리가 이전에 증명한 **단위 계단 함수**의 푸리에 변환을 사용해보자:

$$
U(\omega) = \pi \delta(\omega) + \frac{1}{j\omega}
$$

따라서 $X(\omega) \times U(\omega)$는 다음과 같이 표현할 수 있다:

$$
X(\omega) U(\omega) = \pi \delta(\omega) X(\omega) + \frac{1}{j\omega} X(\omega)
$$

결국, 적분의 푸리에 변환은 곱셈 연산으로 나타낼 수 있으며, **단위 계단 함수**의 푸리에 변환을 이용해 풀 수 있다. 나머지 부분은 직접 계산해보는 것이 좋다.
