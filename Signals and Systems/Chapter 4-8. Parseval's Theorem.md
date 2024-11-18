# Parseval's Theorem

**Parseval's Theorem** states that the total energy of a signal in the time domain is equal to the total energy of the signal in the frequency domain. The theorem is expressed as:

$$
\int_{-\infty}^{\infty} \left| x(t) \right|^2 \, dt = \frac{1}{2\pi} \int_{-\infty}^{\infty} \left| X(\omega) \right|^2 \, d\omega
$$

In this equation, the left side represents the energy of the signal in the time domain, and the right side represents the energy of the signal in the frequency domain. Parseval's theorem states that these two are equal.

### Proof

To prove that the left and right sides are equal, we start by considering the following integral:

$$
\int_{-\infty}^{\infty} x_1(t) x_2^*(t) \, dt
$$

We can express $x_1(t)$ using its **inverse Fourier transform**:

$$
x_1(t) = \frac{1}{2\pi} \int_{-\infty}^{\infty} X_1(\omega) e^{j\omega t} \, d\omega
$$

Similarly, express $x_2^*(t)$ as:

$$
x_2^*(t) = \frac{1}{2\pi} \int_{-\infty}^{\infty} X_2^*(-\omega) e^{j\omega t} \, d\omega
$$

Substitute $-\omega = \omega'$, then $x_2^*(t)$ becomes:

$$
x_2^*(t) = \frac{1}{2\pi} \int_{-\infty}^{\infty} X_2^*(\omega') e^{j\omega' t} \, d\omega'
$$

Now, evaluate the integral $\int_{-\infty}^{\infty} x_1(t) x_2^*(t) \, dt$:

$$
\int_{-\infty}^{\infty} x_1(t) x_2^*(t) \, dt = \frac{1}{4\pi^2} \int_{-\infty}^{\infty} X_1(\omega) \int_{-\infty}^{\infty} X_2^*(\omega') \int_{-\infty}^{\infty} e^{j\omega t} e^{-j\omega' t} \, dt \, d\omega' \, d\omega
$$

The integral of $e^{j\omega t}$ and $e^{-j\omega' t}$ with respect to $t$ is:

$$
\int_{-\infty}^{\infty} e^{j(\omega - \omega') t} \, dt = 2\pi \delta(\omega - \omega')
$$

Thus, the expression simplifies to:

$$
\int_{-\infty}^{\infty} x_1(t) x_2^*(t) \, dt = \frac{1}{2\pi} \int_{-\infty}^{\infty} X_1(\omega) X_2^*(\omega) \, d\omega
$$

If we let $x_2^*(t) = x_1(t)$, Parseval's theorem follows:

$$
\int_{-\infty}^{\infty} \left| x(t) \right|^2 \, dt = \frac{1}{2\pi} \int_{-\infty}^{\infty} \left| X(\omega) \right|^2 \, d\omega
$$

### Conclusion

Parseval's theorem demonstrates the equality of energy in both the time and frequency domains, providing a powerful tool for signal analysis.


# 파시발의 정리

**파시발의 정리**는 시간 영역과 주파수 영역에서 신호의 에너지가 동일하다는 것을 나타내는 중요한 정리다. 이 정리는 다음과 같은 식으로 표현된다:

$$
\int_{-\infty}^{\infty} \left| x(t) \right|^2 \, dt = \frac{1}{2\pi} \int_{-\infty}^{\infty} \left| X(\omega) \right|^2 \, d\omega
$$

위의 식에서 좌변은 시간 영역에서 신호의 에너지를 나타내고, 우변은 주파수 영역에서 신호의 에너지를 나타낸다. 이 둘이 같다는 것이 바로 파시발의 정리이다.

### 증명 과정

좌변과 우변의 식이 같다는 것을 증명하기 위해, 다음 식을 먼저 증명해보자:

$$
\int_{-\infty}^{\infty} x_1(t) x_2^*(t) \, dt
$$

여기서 $x_1(t)$를 **푸리에 역변환**으로 표현하면:

$$
x_1(t) = \frac{1}{2\pi} \int_{-\infty}^{\infty} X_1(\omega) e^{j\omega t} \, d\omega
$$

$x_2^*(t)$도 푸리에 역변환으로 표현하면:

$$
x_2^*(t) = \frac{1}{2\pi} \int_{-\infty}^{\infty} X_2^*(-\omega) e^{j\omega t} \, d\omega
$$

이제 $-\omega = \omega'$라고 치환해보자. 그러면 $x_2^*(t)$는 다음과 같이 변경된다:

$$
x_2^*(t) = \frac{1}{2\pi} \int_{-\infty}^{\infty} X_2^*(\omega') e^{j\omega' t} \, d\omega'
$$

이제 $\int_{-\infty}^{\infty} x_1(t) x_2^*(t) \, dt$를 계산해보자:

$$
\int_{-\infty}^{\infty} x_1(t) x_2^*(t) \, dt = \frac{1}{4\pi^2} \int_{-\infty}^{\infty} X_1(\omega) \int_{-\infty}^{\infty} X_2^*(\omega') \int_{-\infty}^{\infty} e^{j\omega t} e^{-j\omega' t} \, dt \, d\omega' \, d\omega
$$

위의 식에서, $e^{j\omega t}$와 $e^{-j\omega' t}$의 곱에 대해 $t$에 대해 적분하면 다음과 같다:

$$
\int_{-\infty}^{\infty} e^{j(\omega - \omega') t} \, dt = 2\pi \delta(\omega - \omega')
$$

따라서 식은 다음과 같이 단순화된다:

$$
\int_{-\infty}^{\infty} x_1(t) x_2^*(t) \, dt = \frac{1}{2\pi} \int_{-\infty}^{\infty} X_1(\omega) X_2^*(\omega) \, d\omega
$$

여기서 $x_2^*(t)$를 $x_1(t)$로 두면, 파시발의 정리는 다음과 같이 증명된다:

$$
\int_{-\infty}^{\infty} \left| x(t) \right|^2 \, dt = \frac{1}{2\pi} \int_{-\infty}^{\infty} \left| X(\omega) \right|^2 \, d\omega
$$
