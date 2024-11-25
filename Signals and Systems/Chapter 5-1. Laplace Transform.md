# Laplace Transform

What is the **Fourier Transform** we’ve learned so far?

The Fourier series expresses **periodic signals** using complex exponential functions. Then, what concept expresses **non-periodic signals** using complex exponentials?

This is exactly what the **Fourier Transform** does. However, the Fourier Transform has a major limitation: for functions that are **not absolutely integrable**, we must take an alternative approach to represent them. But is this alternative always sufficient?

### Why Laplace Transform?

The Fourier Transform cannot directly handle signals that are **not absolutely integrable**. To address this, the **Laplace Transform** was introduced.

For example, the following function is not absolutely integrable and thus cannot be transformed using the Fourier Transform:

$$
h(t) = e^{3t}u(t)
$$

What happens if we multiply $h(t)$ by $e^{-\sigma t}$ and then apply the Fourier Transform?

### The Role of $e^{-\sigma t}$

Let’s first examine the behavior of $e^{-\sigma t}$:

1. When $\sigma > 0$:
    
    ![sigma](https://i.imgur.com/3ocl83Z.png)
    
2. When $\sigma < 0$:
    
    ![sigma](https://i.imgur.com/9bi8pEo.png)
    
By choosing $\sigma > 0$, $e^{-\sigma t}$ exponentially decreases the magnitude of the signal, allowing previously non-integrable signals to become integrable.

### Definition of the Laplace Transform

If we multiply $h(t)$ by $e^{-\sigma t}$ and then apply the Fourier Transform, we obtain a **two-variable function**:

$$
h(t)e^{-\sigma t} \xleftrightarrow{\mathcal{F}} H(\sigma, \omega)
$$

For simplicity, we represent this two-variable function as a single variable. The Laplace Transform is defined as follows:

$$
H(\sigma, \omega) = \int_{0}^{\infty} h(t)e^{-\sigma t}e^{-j\omega t}dt
$$

Simplifying:

$$
H(\sigma, \omega) = \int_{0}^{\infty} h(t)e^{-(\sigma + j\omega)t}dt
$$

If we substitute $\sigma + j\omega = s$, the equation reduces to:

$$
H(s) = \int_{0}^{\infty} h(t)e^{-st}dt
$$

### Key Features of the Laplace Transform

- The result of the Laplace Transform is expressed in terms of the **complex variable $s$**.
- The **inverse Laplace Transform** is computationally complex, so it’s often done using precomputed tables or software.
- Depending on the value of $s$, a signal may **converge** or **diverge**. This defines the **Region of Convergence (ROC)**.
- The ROC depends on the given signal and must be calculated specifically for each case.




# 라플라스 변환

우리가 기존에 배웠던 **푸리에 변환**은 무엇인가? 

푸리에 급수는 **주기 신호**를 복소 지수함수로 표현하고자 하는 개념이었다. 그렇다면 **주기 신호가 아닌 신호**를 복소 지수함수로 표현하려는 개념은 무엇일까? 

바로 **푸리에 변환**이다. 하지만 푸리에 변환에는 큰 한계가 있다. **절대 적분이 불가능한 함수**의 경우, 이를 표현하기 위해 우회해야 한다는 것이다. 하지만 이런 우회 방식이 과연 적절한 방법일까?

### 라플라스 변환의 필요성

푸리에 변환은 **절대 적분이 불가능한 신호**를 직접 다룰 수 없다. 이 문제를 해결하기 위해 **라플라스 변환**이 도입되었다.

예를 들어, 아래와 같은 함수는 절대 적분이 불가능하므로 푸리에 변환을 바로 적용할 수 없다:

$$
h(t) = e^{3t}u(t)
$$

이때 $h(t)$에 $e^{-\sigma t}$를 곱한 형태를 푸리에 변환하면 어떻게 될까?

### $e^{-\sigma t}$의 역할

먼저 $e^{-\sigma t}$의 개형을 살펴보자:

1. $\sigma > 0$의 경우:
    
    ![sigma](https://i.imgur.com/3ocl83Z.png)
    
2. $\sigma < 0$의 경우:
    
    ![sigma](https://i.imgur.com/9bi8pEo.png)
    
$\sigma$를 양수로 잡으면 $e^{-\sigma t}$는 신호의 크기를 빠르게 줄인다. 이를 통해 원래 적분이 불가능했던 신호도 적분 가능하게 만들 수 있다.

### 라플라스 변환의 정의

$h(t)e^{-\sigma t}$를 푸리에 변환하면 다음과 같은 이변수 함수가 된다:

$$
h(t)e^{-\sigma t} \xleftrightarrow{\mathcal{F}} H(\sigma, \omega)
$$

이 이변수 함수를 **단일 변수**로 표현하면 더 편리할 것이다. 이를 위해 다음과 같이 정의한다:

$$
H(\sigma, \omega) = \int_{0}^{\infty} h(t)e^{-\sigma t}e^{-j\omega t}dt
$$

이를 정리하면:

$$
H(\sigma, \omega) = \int_{0}^{\infty} h(t)e^{-(\sigma + j\omega)t}dt
$$

여기서 $\sigma + j\omega = s$로 치환하면, 식은 다음과 같이 단순화된다:

$$
H(s) = \int_{0}^{\infty} h(t)e^{-st}dt
$$

### 라플라스 변환의 특징

- 라플라스 변환의 결과는 **$s$라는 복소수 변수**로 표현된다.
- 라플라스 변환의 **역변환**은 계산이 복잡하므로, 주로 테이블을 참고하여 암기하거나 변환을 직접 수행한다.
- $s$ 값에 따라 신호가 **수렴**하거나 **발산**할 수 있다. 이를 **수렴 영역(ROC, Region of Convergence)** 라고 한다.
- 수렴 영역은 주어진 신호에 따라 달라지며, 이를 직접 계산해 찾을 수 있다.











