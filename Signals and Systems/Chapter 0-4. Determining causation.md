# English

### Causality Determination

To determine whether a system is causal, we examine the relationship between the input function $x(t)$ and the output function $y(t)$. A system is causal if the output at any time depends only on the current and past inputs, not on future inputs. If the output depends on future inputs, the system is non-causal.

Let's go through some examples.

1. **$y(t) = x(3t)$**

To check for causality, we can substitute a specific value, such as $t = 1$:

$$
y(1) = x(3)
$$

This situation is represented in the following graph:

![causal](https://i.imgur.com/8gJ7l1T.png)

Here, the input occurs at $t = 3$, but the output occurs at $t = 1$. Since the output precedes the input, this system is non-causal.

2. **$y(t) = x(t) \cos(t+1)$**

Let's substitute $t = 1$ into the equation:

$$
y(1) = x(1) \cos(2)
$$

Initially, you might think that because there is a factor of $t + 1$, the system could be non-causal. However, causality is determined by the relationship between $x(t)$ and $y(t)$ alone. The cosine term does not affect causality, as it only scales the output. Since $y(t)$ depends on $x(t)$ at the same time $t$, the system is causal.

Thus, the relationship $x(\alpha)$ and $y(\beta)$ is causal if $\alpha \leq \beta$. If the reverse is true, the system is non-causal.

However, there are cases where this rule might lead to confusion.

3. **$y(t) = x(-t)$**

For this relationship, if we substitute $t = 1$, we get:

$$
y(1) = x(-1)
$$

Here, the input occurs at $t = -1$, and the output occurs at $t = 1$. This might seem causal at first, but if we consider $t = -1$, the output is:

$$
y(-1) = x(1)
$$

In this case, the input occurs after the output, making the system non-causal. Therefore, when dealing with negative time shifts, it's essential to carefully examine the system with different values to accurately determine causality.


# korean

### Causal 판단하기

입력 함수인 $x(t)$와 출력 함수인 $y(t)$의 관계를 통해 시스템이 causal인지 판단할 수 있다. 시스템이 causal이라는 것은 출력이 현재와 과거의 입력에만 의존하고, 미래의 입력에는 의존하지 않는다는 의미다. 반대로, 출력이 미래의 입력에 의존하면 시스템은 non-causal이다.

몇 가지 예제를 통해 살펴보자.

1. **$y(t) = x(3t)$**

Causal 여부를 확인하기 위해 $t = 1$을 대입해 보자:

$$
y(1) = x(3)
$$

이 상황은 다음 그래프로 표현할 수 있다:

![causal](https://i.imgur.com/8gJ7l1T.png)

여기서 입력은 $t = 3$에서 발생하지만 출력은 $t = 1$에서 발생한다. 출력이 입력보다 먼저 발생하므로, 이 시스템은 non-causal이다.

2. **$y(t) = x(t) \cos(t+1)$**

이번에도 $t = 1$을 대입해 보자:

$$
y(1) = x(1) \cos(2)
$$

처음에는 $t+1$이라는 항 때문에 시스템이 non-causal일 수도 있다고 생각할 수 있다. 그러나 causal 여부는 $x(t)$와 $y(t)$의 관계에 따라 결정된다. 코사인 항은 출력만을 스케일링할 뿐, causal 여부에는 영향을 미치지 않는다. $y(t)$가 $x(t)$와 같은 시간 $t$에 의존하므로, 이 시스템은 causal이다.

즉, $x(\alpha)$와 $y(\beta)$의 관계에서 $\alpha \leq \beta$이면 causal이며, 그렇지 않으면 non-causal이라고 생각할 수 있다.

그러나 이에 대해 모순이 생기는 경우도 있다.

3. **$y(t) = x(-t)$**

이 관계에서 $t=1$을 넣어 비교한 결과는 $y(1) = x(-1)$이다. 즉, 입력 시간은 $-1$이고 출력 시간은 $1$이다. 이때는 causal처럼 보이지만, 시간이 $t=-1$이라면 반대로 $y(-1) = x(1)$이므로 non-causal이 된다. 즉, 음수가 들어간 식에서는 함부로 판단하면 안 되며, 여러 수를 넣어 판단하는 과정이 반드시 필요하다.


