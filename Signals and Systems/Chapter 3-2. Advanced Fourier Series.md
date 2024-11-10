# Advanced Fourier Series

This chapter aims to answer the two questions posed in the introduction to Fourier series:

- Can every periodic function be represented?
- Is there a one-to-one correspondence?

To answer these questions, we first need to consider the following:

$$
e^{jk \omega_0 t}
$$

Is the above complex exponential function a vector?

Yes, it is! We now move beyond Euclidean vector spaces and consider general vector spaces.

In fact, any element of a vector space is called a vector. So, what is a **vector space**?

A vector space is a set that is closed under vector addition and scalar multiplication and satisfies 8 axioms. This concept is studied in detail in linear algebra.

To include the function above in a set, we consider a set that satisfies the following operation:

$$
k_1' e^{jk_1 \omega_0 t} + k_2' e^{jk_2 \omega_0 t}
$$

A set that satisfies such operations can include the following expression:

$$
\sum_{-\infty}^{\infty} a_k e^{jk\omega_0 t}
$$

If inner products are defined in this vector space, we can consider additional concepts such as **length** and **angle**.

With this in mind, let’s define an inner product as follows:

$$
\langle a(t), b(t) \rangle \triangleq \int_{T_0} a(t) \, b^*(t) \, dt 
$$

You might wonder why we use this definition, but we are dealing with a general vector space, not just Euclidean space. This definition was found through extensive trials.

Like in usual inner products, if the result is $0$, the vectors are orthogonal.

For example:

$$
\langle e^{jk\omega_0 t}, e^{jr\omega_0 t} \rangle = \int_{T_0} e^{j(k-r)\omega_0 t} \, dt
$$

$$
= \int_{T_0} \cos((k-r)\omega_0 t) + j\sin((k-r)\omega_0 t) \, dt
$$

$$
= \begin{cases}
0 & \text{if } k \neq r \\
T_0 & \text{if } k = r
\end{cases}
$$

Thus, $\sum_{-\infty}^{\infty} a_k e^{jk\omega_0 t}$ is a linear combination where the vectors are orthogonal and linearly independent, forming an infinite-dimensional space.

Let’s revisit our initial questions:

Can every periodic function be represented?

Most periodic functions can be represented. However, if a function does not fit the linear combination structure we defined, it cannot be represented. Fortunately, this rarely happens.

Is there a one-to-one correspondence?

Yes, if the period $T_0$ is known. We need to know the period for a one-to-one correspondence to exist.

Finally, why do we only use Harmonics? There is no need to use non-integer multiples since the set size is already large, and using real multiples would not provide significant improvement.

With these concepts understood, we can now derive Fourier coefficients and interpret them using inner products. Let’s move on after a thorough review.



# 푸리에 급수 심화

푸리에 급수 기초에서 던진 두 가지 질문이 있다. 이 질문을 해결하기 위한 챕터라고 생각하면 된다.

- 모든 주기 함수에서 표현 가능한가?
- 일대일 대응인가?

위의 질문을 해결하기 위해 먼저 생각해야 할 부분이 있다.

$$
e^{jk \omega_0 t}
$$

위의 복소 지수함수는 벡터일까?

벡터이다! 우리는 더 이상 유클리드 벡터 공간만을 상정하여 말하지 않고, 일반 벡터 공간을 생각해야 한다.

애초에 벡터 공간 안의 원소를 우리는 벡터로 칭하기 때문이다. **벡터 공간**이란?

8개의 공리를 만족하는 벡터합과 스칼라 곱에 대해 닫혀 있는 집합을 우리는 벡터 공간이라 표현한다. 이 개념은 선형대수학에서 자세히 배운다.

위의 함수를 하나의 집합에 넣기 위해 다음 연산을 만족하는 집합을 상정해보자.

$$
k_1' e^{jk_1 \omega_0 t} + k_2' e^{jk_2 \omega_0 t}
$$

이러한 연산들을 만족하는 set이라 해보자. 그렇다면 당연하게 다음 표현들은 전부 set에 포함될 수 있다.

$$
\sum_{-\infty}^{\infty} a_k e^{jk\omega_0 t}
$$

위의 벡터 공간에서 **내적**(inner product)까지 연산이 정의된다면, 우리는 더 많은 개념을 다룰 수 있게 된다.

바로, **길이**와 **각도**를 표현할 수 있게 된다!

위의 생각을 바탕으로, 우리는 내적을 다음과 같이 정의해보자.

$$
\langle a(t), b(t) \rangle \triangleq \int_{T_0} a(t) \, b^*(t) \, dt 
$$

물론 이 글을 읽는 독자들이 "왜 이런 내적 정의를 사용하는가?"에 대해 의심할 수 있지만, 우리는 유클리드 공간에서 벗어나 일반 벡터 공간을 다루고 있으므로, 임의의 내적 정의가 이상해 보여도 당연하게 받아들여야 한다. 위의 정의도 사실 여러 시도 끝에 얻어낸 결과이다.

위의 정의에서도 일반적인 내적과 마찬가지로, 값이 $0$이 된다면 두 벡터가 수직임을 의미한다.

예를 들어보자:

$$
\langle e^{jk\omega_0 t}, e^{jr\omega_0 t} \rangle = \int_{T_0} e^{j(k-r)\omega_0 t} \, dt
$$

$$
= \int_{T_0} \cos((k-r)\omega_0 t) + j\sin((k-r)\omega_0 t) \, dt
$$

$$
= \begin{cases}
0 & \text{if } k \neq r \\
T_0 & \text{if } k = r
\end{cases}
$$

즉, 위의 정의에 의해 $\sum_{-\infty}^{\infty} a_k e^{jk\omega_0 t}$는 모두 선형 결합(linear combination)이며, 각 벡터는 직교하고, 선형 독립임을 알 수 있다. 이는 차원이 $\infty$인 공간이다.

이래서 우리가 내적의 개념을 다시 살펴본 것이다.

이제, 해결하려는 질문을 다시 보자. 두 질문에 대한 답변은 대부분 "맞다"라고 할 수 있으나, 항상 맞는 것은 아니다.

모든 주기 함수를 표현할 수 있을까?

우리가 생각할 수 있는 대부분의 주기 함수는 표현할 수 있다. 하지만 우리가 집합을 선형 결합으로 구성했기 때문에, 이 조건을 만족하지 않는 함수는 표현할 수 없다. 그러나 대부분의 주기 함수는 표현 가능하므로 너무 걱정할 필요는 없다.

또한, 일대일 대응이 가능한가?

주기 $T_0$가 주어진 경우, 일대일 대응이 가능하다. 즉, 주기를 알아야만 일대일 대응이 성립한다는 것이다.

마지막으로, 왜 **Harmonics**만을 사용할까? 정수 배가 아닌 신호를 굳이 사용할 필요가 없기 때문이다. 이미 집합의 크기가 충분히 크고, 실수 배를 사용해도 약간의 개선은 있겠지만 큰 차이가 없으므로 정수 배만을 사용하는 것이다.

이제 위의 개념들을 바탕으로 푸리에 계수를 유도하고, 내적으로 이를 해석해볼 것이다. 잘 복습하고 다음으로 넘어가자.

