# Fourier Transform of Differentiation

We previously derived the **Fourier Transform** formula as follows:

$$
x(t) = \frac{1}{2\pi} \int_{-\infty}^{\infty} X(\omega) e^{j\omega t} \, d\omega
$$

Now, what happens if we **differentiate** $x(t)$?

We could find $\frac{d}{dt} x(t)$ using techniques like integration by parts, but instead, we’ll directly state the result:

$$
\frac{d}{dt} x(t) = \frac{1}{2\pi} \int_{-\infty}^{\infty} j\omega X(\omega) e^{j\omega t} \, d\omega
$$

This shows a relationship between $\frac{d}{dt} x(t)$ and $j\omega X(\omega)$.

Next, we need to find **$h(t)$**, the function that, when convolved with $x(t)$, produces $y(t)$. Using the properties of the Fourier Transform, we know that convolution in time domain corresponds to multiplication in the frequency domain:

$$
Y(\omega) = H(\omega) X(\omega)
$$

To find $h(t)$, we determine $\frac{Y(\omega)}{X(\omega)}$ and then take the **inverse Fourier Transform**. Let’s solve an example differential equation:

$$
y' + 2y = 3x' + x
$$

Taking the **Fourier Transform** of the equation, we get:

$$
j\omega Y(\omega) + 2Y(\omega) = 3j\omega X(\omega) + X(\omega)
$$

Rewriting this in the form $\frac{Y(\omega)}{X(\omega)}$:

$$
H(\omega) = \frac{Y(\omega)}{X(\omega)} = \frac{3(2 + j\omega) - 5}{2 + j\omega} = 3 - \frac{5}{2 + j\omega}
$$

Finally, the **inverse Fourier Transform** of $H(\omega)$ is:

$$
\mathcal{F^{-1}}\{H(\omega)\} = \mathcal{F^{-1}}\left(3-\frac{5}{2+j\omega}\right) = 3\delta(t) - 5e^{-2t}u(t)
$$

This demonstrates that the differential equation can be **easily solved** using the Fourier Transform.


# 미분의 푸리에 변환

다음과 같은 **푸리에 변환 공식**을 우리는 쉽게 구했었다:

$$
x(t) = \frac{1}{2\pi} \int_{-\infty}^{\infty} X(\omega) e^{j\omega t} \, d\omega
$$

그렇다면, $x(t)$를 **미분**한 꼴은 어떻게 될까?

${d\over dt} x(t)$는 부분적분 등의 계산법을 통해 구할 수 있지만, 여기서는 계산보다는 결과를 중점으로 보겠다:

$$
\frac{d}{dt} x(t) = \frac{1}{2\pi} \int_{-\infty}^{\infty} j\omega X(\omega) e^{j\omega t} \, d\omega
$$

즉, $\frac{d}{dt} x(t)$와 $j\omega X(\omega)$의 관계를 나타낸 것이다.

이제 우리는 **$h(t)$**를 찾아야 한다. 여기서 $h(t)$는 $x(t)$와 **컨볼루션** 계산을 진행하는 함수이며, 결과로 $y(t)$가 나온다. 푸리에 변환의 특성에 따라, 컨볼루션 계산 결과는 곱셈으로 표현되며, 다음과 같이 나타낼 수 있다:

$$
Y(\omega) = H(\omega) X(\omega)
$$

우리가 구해야 할 $h(t)$를 찾기 위해 $\frac{Y(\omega)}{X(\omega)}$를 구하고, 이를 **역 푸리에 변환**하면 된다. 예를 들어, 다음과 같은 미분 방정식을 풀어야 한다고 가정해보자:

$$
y' + 2y = 3x' + x
$$

이 방정식은 다음과 같이 **푸리에 변환**할 수 있다:

$$
j\omega Y(\omega) + 2Y(\omega) = 3j\omega X(\omega) + X(\omega)
$$

이를 $\frac{Y(\omega)}{X(\omega)}$ 형태로 나타내면:

$$
H(\omega) = \frac{Y(\omega)}{X(\omega)} = \frac{3(2 + j\omega) - 5}{2 + j\omega} = 3 - \frac{5}{2 + j\omega}
$$

이제, $H(\omega)$를 **역 푸리에 변환**하면 다음과 같다:

$$
\mathcal{F^{-1}}\{H(\omega)\} = \mathcal{F^{-1}}\left(3-\frac{5}{2+j\omega}\right) = 3\delta(t) - 5e^{-2t}u(t)
$$

따라서, 미분 방정식이 **쉽게 풀림**을 알 수 있다.


