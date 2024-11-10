## Dirichlet Conditions

We defined the function $x_{T_0}(t)$ as follows:

$$
x_{T_0}(t) = \sum_{-\infty}^{\infty} a_k e^{jk\omega_0 t}
$$

This function assumes an **infinite sum**. However, we can also consider a finite case, which can be represented as:

$$
\hat{x}_{T_0}(t) = \sum_{k=-N}^{N} a_k e^{jk\omega_0 t}
$$

Subtracting the energy expression of this finite approximation from the original function’s energy expression, we get:

$$
\int_{T_0} \left| x_{T_0}(t) - \hat{x}_{T_0}(t) \right|^2 \, dt
$$

If $N \to \infty$, the result of this integral becomes $0$. This means the two functions are equal.

Is it possible for the functions to be equal without $N \to \infty$?

The answer lies in satisfying the **Dirichlet Conditions**:

1. $\int_{T_0} \left| x_{T_0}(t) \right| \, dt < \infty$: The function must be **absolutely integrable**.
2. The **minimum (min)** and **maximum (max)** values of the function must be finite.
3. The function must have a **finite number of discontinuities**.

Remember these 3 conditions as they are crucial for ensuring the validity of the Fourier series representation.

## 디리클레 조건

우리가 함수 $x_{T_0}(t)$를 다음과 같이 정의했었다.

$$
x_{T_0}(t) = \sum_{-\infty}^{\infty} a_k e^{jk\omega_0 t}
$$

위의 함수는 **무한 합**을 상정하고 만들어진 꼴이다. 하지만, 유한한 경우도 고려할 수 있다. 이를 다음과 같이 표현해보자.

$$
\hat{x}_{T_0}(t) = \sum_{k=-N}^{N} a_k e^{jk\omega_0 t}
$$

이제, 원래 함수의 에너지 식에서 위의 유한 합으로 정의한 함수의 에너지 식을 빼면 다음과 같은 형태가 된다:

$$
\int_{T_0} \left| x_{T_0}(t) - \hat{x}_{T_0}(t) \right|^2 \, dt
$$

만약 $N \to \infty$라면, 이 식의 값은 $0$이 된다. 즉, 두 함수가 같아진다는 의미이다.

그러면 $N \to \infty$이 아닐 때에도 두 함수가 같을 수 있는 조건이 있을까?

이를 만족하는 식이 바로 **디리클레 조건**이다:

1. $\int_{T_0} \left| x_{T_0}(t) \right| \, dt < \infty$: 즉, 함수는 절대 적분이 가능해야 한다.
2. 함수의 **최솟값(min)**과 **최댓값(max)**이 유한해야 한다.
3. **불연속점(discontinuity)**이 유한해야 한다.

위의 3가지 조건을 잘 기억하고 넘어가자.

