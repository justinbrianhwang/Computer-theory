# Deriving Fourier Coefficients & Interpreting with Inner Product

Although we have discussed the Fourier series in detail, we haven’t yet mentioned the **coefficients**. Let’s derive them now.

$$
x_{T_0}(t) = \sum_{k=-\infty}^{\infty} a_k e^{jk\omega_0 t}
$$

Now, multiply both sides by $e^{-jr\omega_0 t}$ and take the inner product.

$$
\int_{T_0} x_{T_0}(t) e^{-jr\omega_0 t} \, dt = \int_{T_0} \sum_{k=-\infty}^{\infty} a_k e^{j(k-r)\omega_0 t} \, dt
$$

From the above operation, we can extract the **Fourier coefficients** $a_k$ as follows:

$$
a_k = \frac{1}{T_0} \int_{T_0} x_{T_0}(t) e^{-jk\omega_0 t} \, dt
$$

While memorizing this formula is useful, understanding its **interpretation** is more important.

Rewriting the expression in terms of an inner product, we get:

$$
a_k = \frac{1}{T_0} \langle x_{T_0}(t), e^{jk\omega_0 t} \rangle
$$

This means that $a_k$ is the **inner product** of $x_{T_0}(t)$ and $e^{jk\omega_0 t}$. Visually, we can illustrate this for $k=2$ and $k=3$ as follows:

![inner](https://i.imgur.com/ZQ9EhV6.png)

By expressing it as an inner product, we can see how much each vector (basis function) contributes to the signal. A larger inner product value indicates a stronger relationship between the vectors.


# 푸리에 계수 유도 & 내적으로 해석하기

우리가 계속해서 푸리에 급수에 대해서 다루었지만, **계수**에 대해서는 언급하지 않았다. 이제 푸리에 계수를 어떻게 구하는지 살펴보자.

$$
x_{T_0}(t) = \sum_{k=-\infty}^{\infty} a_k e^{jk\omega_0 t}
$$

이제, 위의 함수에 양변에 $e^{-jr\omega_0 t}$를 곱하고 내적을 해보자.

$$
\int_{T_0} x_{T_0}(t) e^{-jr\omega_0 t} \, dt = \int_{T_0} \sum_{k=-\infty}^{\infty} a_k e^{j(k-r)\omega_0 t} \, dt
$$

위의 연산 결과를 보면, 다음과 같이 **푸리에 계수** $a_k$를 뽑아낼 수 있다.

$$
a_k = \frac{1}{T_0} \int_{T_0} x_{T_0}(t) e^{-jk\omega_0 t} \, dt
$$

이렇게 계수를 유도해낸 것이다. 사실, 위의 식을 외우는 것도 좋지만, 그 **해석**을 이해할 줄 알아야 한다.

위의 식을 내적 꼴로 적절히 변형하면 다음과 같이 표현할 수 있다.

$$
a_k = \frac{1}{T_0} \langle x_{T_0}(t), e^{jk\omega_0 t} \rangle
$$

즉, 위의 식은 $x_{T_0}(t)$와 $e^{jk\omega_0 t}$의 **내적값**을 의미한다. 이를 그림으로 표현하면 다음과 같다. 여기서는 임의로 $k=2$와 $k=3$만 예시로 살펴보겠다.

![inner](https://i.imgur.com/ZQ9EhV6.png)

이처럼 내적으로 표현함으로써, 각 벡터 간의 연관성을 파악할 수 있게 된다. 벡터 간 내적값이 클수록 두 벡터가 서로 유사하다는 것을 의미한다.





