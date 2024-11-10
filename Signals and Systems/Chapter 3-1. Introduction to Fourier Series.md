

# Introduction to Fourier Series

The term "series" might sound familiar. In calculus, we often encounter the **Taylor series**, so before discussing the Fourier series, let’s quickly review the Taylor series.

### Taylor Series

Simply put, the Taylor series represents a transcendental function as a polynomial! The concept begins with the idea that any function can be represented in the following form:

$$
f(x) = c_0 + c_1 x + c_2 x^2 + \cdots
$$

In particular, if the series is centered at $x = 0$, we call it the **Maclaurin series**. The Taylor series allows us to simplify complex integrals and perform calculations more easily, making it a valuable tool.

Now, let’s explore what the **Fourier series** is about.

### Fourier Series

The Fourier series approximates periodic signals (periodic functions). The key idea is that periodic functions can be expressed using sinusoidal functions.

$$
x_{T_0 } (t) = \cdots + a_{-2} e^{j(-2)\omega_0 t} + a_{-1} e^{j(-1)\omega_0 t} + a_0 + a_{1} e^{j(1)\omega_0 t} + a_{2} e^{j(2)\omega_0 t} + \cdots
$$

Before we proceed with complex exponential functions, let’s first consider the concept behind it. Take a look at the following diagram:

![euler](https://i.imgur.com/T0AmcPE.png)

The image above represents the function $e^{j2\pi t}$, which completes one full rotation per second. So, how many rotations per second does the function $e^{j2\pi f_0 t}$ complete?

It completes $f_0$ rotations per second!

Thus, in the expression above, $\omega_0$ represents $\omega_0 = 2\pi f_0$. We only consider integer multiples of the fundamental frequency, which are called **Harmonics**.

When dealing with complex exponential functions, one might ask whether these functions can accurately represent real-valued signals.

By appropriately choosing the coefficients and summing the terms, we can eliminate the imaginary parts and effectively represent any periodic signal!

To see how well this representation works, take a look at the following diagram:

![gibb](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEiKs4H4xa1EorPcoMLh87L9wW0ne628NGX4I4QJltgsRjtaSUtGFDE3rGc4gr4rKbyvlP24a4UmTy-n1BRuw1hMWg7Vq6Q31K6CVYQZ38gNKLXbWa1JOGSRRCQWFL2GaU8EUR7J4vjHI0nEO4pYbqa8nMk5MPAB6eaqX9yOCkrFZlSglcjdnNpr7w4vvw/s16000/gp1.png)

The diagram shows how closely the approximation gets as more terms are added. However, there is a portion that does not decrease, known as the **Gibbs phenomenon**.

Finally, we are left with two fundamental questions about Fourier series:

- Can we represent every periodic function?
- Is there a one-to-one correspondence?

To answer these questions, we need to delve deeper.



# 푸리에 급수 기초

‘급수’라는 용어는 많이 들어봤을 법한 용어이다. 미적분학에서 접하는 **테일러 급수**가 익숙할 테니, 푸리에 급수를 말하기 전, 테일러 급수를 먼저 복습하도록 하자.

### 테일러 급수

테일러 급수를 단순하게 말하면, 초월함수를 다항함수로 표현한 것이다! 즉 아래와 같은 형태로 모든 함수를 표현할 수 있다는 것에서 시작된 개념인 것이다.

$$
f(x) = c_0 + c_1 x + c_2 x^2 + \cdots
$$

특히, $x = 0$인 곳에서 테일러 급수를 표현한 위와 같은 식을 우리는 **매클로린 급수**라 칭한다. 테일러 급수를 통해 우리는 표현하기 어려웠던 적분 표현도 쉽게 표현이 가능해지고, 여러 연산에서 이점을 얻었기에 사용하던 개념이었다.

그렇다면 우리가 앞으로 다룰 **푸리에 급수**는 어떤 개념인지 살펴보도록 하자.

### 푸리에 급수

푸리에 급수란, 주기 신호(주기 함수)를 근사 표현한 것이다. 특히 주기 함수는 정현파로 표현할 수 있다는 점을 이용할 것이다.

$$
x_{T_0 } (t) = \cdots + a_{-2} e^{j(-2)\omega_0 t} + a_{-1} e^{j(-1)\omega_0 t} + a_0 + a_{1} e^{j(1)\omega_0 t} + a_{2} e^{j(2)\omega_0 t} + \cdots
$$

우리가 복소 지수함수로 표현할 때, 생각해야 할 개념이 있다. 아래의 그림을 먼저 보도록 하자.

![euler](https://i.imgur.com/T0AmcPE.png)

위의 그림을 $e^{j2\pi t}$ 함수를 표현한 그림이라고 할 때, 1초에 한 바퀴 회전한다는 의미로 받아들이자. 그렇다면 $e^{j2\pi f_0 t}$ 함수라면 1초에 몇 바퀴 회전할까?

$f_0$ 바퀴 회전하는 것이다!

즉 위에서 표현된 함수에서, $\omega_0$는 $\omega_0 = 2\pi f_0$를 의미한다! 기본 주파수의 정수 배수만을 채택했으며, 이 정수 배수를 우리는 **Harmonics**라 한다.

복소 지수 함수를 다루면서, 과연 복소 지수함수가 실수 신호를 표현하기에 적절할까?

계수와 적절한 합을 통해 복소수 부분을 소거할 수 있어, 모든 주기 신호를 적절하게 표현할 수 있는 것이다!

아래의 그림을 통해 실제 표현이 잘 되었는지 확인해보자.

![gibb](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEiKs4H4xa1EorPcoMLh87L9wW0ne628NGX4I4QJltgsRjtaSUtGFDE3rGc4gr4rKbyvlP24a4UmTy-n1BRuw1hMWg7Vq6Q31K6CVYQZ38gNKLXbWa1JOGSRRCQWFL2GaU8EUR7J4vjHI0nEO4pYbqa8nMk5MPAB6eaqX9yOCkrFZlSglcjdnNpr7w4vvw/s16000/gp1.png)

위의 그림은 더한 항의 수에 따라 얼마나 정확히 근사할 수 있는지를 보여준다. 다만 줄어들지 않는 부분을 **깁스 현상**이라 부른다.

마지막으로, 우리는 푸리에 급수에서 두 가지 의문점을 가질 수 있다:

- 모든 주기함수를 표현할 수 있는가?
- 일대일 대응이 가능한가?

위의 두 질문을 해결하기 위해, 우리는 좀 더 깊게 들어갈 것이다.

