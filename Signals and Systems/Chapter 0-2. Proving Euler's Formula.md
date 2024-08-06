# English

### Proof of Euler's Formula

We will now prove Euler's formula, which is a prerequisite in signals and systems.

Let's look at Euler's formula.

$$
e^{jx} = \cos x + j\sin x
$$

Here, $j$ represents the number $\sqrt{-1}$. In calculus or higher mathematics, it is denoted by $i$, but in signals and systems, it is denoted by $j$ to avoid confusion with current.

At first glance, the above formula might seem confusing. Let's recall the Maclaurin series we learned in calculus, which is the Taylor series at $x=0$. We will express the Maclaurin series for the basic functions $e^x,~\sin x,~\cos x$.

$$
e^x = \sum_{k=0}^{\infty} \frac{1}{k!} x^k 
$$

$$
\sin x = \sum_{k=0}^{\infty} \frac{(-1)^k}{(2k+1)!} x^{2k+1} 
$$

$$
\cos x = \sum_{k=0}^{\infty} \frac{(-1)^k}{(2k)!} x^{2k} 
$$

These series should be familiar to students who have studied calculus. Now, let's use them to express $e^{jx}$.

$$
e^{jx} = \sum_{k=0}^{\infty} \frac{1}{k!} (jx)^k 
$$

Expanding the series and separating terms for even and odd $k$, we get:

$$
1 - \frac{1}{2!} x^2 + \frac{1}{4!} x^4 - \cdots + jx - j\frac{1}{3!} x^3 + \cdots 
$$

$$
= \cos x + j \sin x
$$

As we can see, this confirms the formula.


# Korean

### 오일러 포뮬러 증명

앞으로 신호 및 시스템의 전제조건 중 하나인 오일러 포뮬러를 증명할 것이다. 

오일러 포뮬러를 보자.

$$
e^{jx} = \cos x + j\sin x
$$

이때, $j$는 $\sqrt{-1}$인 수를 의미한다. 참고로, 미적분학이나, 고등수학에서는 $i$로 표기하지만, 신호 및 시스템에서는 전류를 의미하기도 하므로 혼동을 방지하기 위해 $j$로 표기할 것이다.

위의 공식을 보면 왜 저렇게 나온지 이해가 안갈 수 있다. 먼저, 우리가 미적분학에서 배운 매클로린 급수를 떠올려보자. $x=0$에서 테일러 급수를 의미한다. 기본 함수인, $e^x,~\sin x, ~\cos x$의 매클로린 급수를 각각 표현해보자.

$$
e^x = \sum_{k=0}^{\infty} \frac{1}{k!} x^k 
$$

$$
\sin x = \sum_{k=0}^{\infty} \frac{(-1)^k}{(2k+1)!} x^{2k+1} 
$$

$$
\cos x = \sum_{k=0}^{\infty} \frac{(-1)^k}{(2k)!} x^{2k} 
$$

위의 식은 미적분학을 다룬 학생들이라면 누구나 이해할 급수들이다. 이를 이용해서 $e^{jx}$를 표현해보자.

$$
e^{jx} = \sum_{k=0}^{\infty} \frac{1}{k!} (jx)^k 
$$

위의 식에서 풀어서 써본 뒤 $k$가 짝수일 때와 홀수 일때를 각각 표현해보면,

$$
1 - \frac{1}{2!} x^2 + \frac{1}{4!} x^4 - \cdots + jx - j\frac{1}{3!} x^3 + \cdots 
$$

$$
= \cos x + j \sin x
$$

임을 우리가 확인할 수 있다.

