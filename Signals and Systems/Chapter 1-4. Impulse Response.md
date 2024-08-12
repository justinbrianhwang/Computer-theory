# English

Understanding $h(t)$ well essentially means understanding the system itself.

### Memoryless System

We've studied $h(t)$ to understand what the system represents. The interpretation of $h(t)$ can vary depending on its range. The following diagram will help clarify this concept:

![memory](https://i.imgur.com/ZpdJewU.png)

The different regions can be analyzed as follows:

**Before Input**: If a response occurs before the input is applied, it implies a reaction to a future signal.

**After Input**: If a response occurs after the input, it indicates a reaction to a past signal.

So, what is a Memoryless System? A memoryless system is one where the output response occurs only at the moment of the input and not beyond that.

Additionally, a causal system is one where the output depends on past and present inputs. In other words, the system responds only at the moment the input is received and after the input has been applied.

### Stable (BIBO Stable) System

To understand this system, it's helpful to refer to the following diagram:

![Bibo stable](https://i.imgur.com/QbIQVjS.png)

The basic condition for a BIBO (Bounded Input, Bounded Output) Stable system is convergence:

$$|y(t)| = | \int x(\tau) h(t - \tau) d\tau | \leq \int |x(\tau) h(t - \tau)| d\tau$$  

$$= \int |x(\tau) h(t - \tau)| d\tau$$ (For all complex numbers)

If $$\int |h(t)| dt$$ converges, let's denote this as $B$.

$$ \int |x(\tau) h(t - \tau)| d\tau < B \int |h(t - \tau)| d\tau$$ (Converges)

Since a larger function converges, $y(t)$ also converges.



# Korean

$h(t)$를 잘 안다는 의미는, 결국 그 시스템을 잘 안다는 의미이다. 

### Memoryless system

사실 우리는 그동안 $h(t)$를 공부했다. 공부한 이유는 해당 시스템이 어떤 의미를 가지고 있는지 파악하기 위함이다. $h(t)$의 범위에 따라 다르게 파악할 수 있다. 

다음 그림을 보면 더욱 이해가 쉬울 것이다. 

![memory](https://i.imgur.com/ZpdJewU.png)

각각의 영역을 분석하면 다음과 같다. 

**입력 전**: 입력이 들어가기 전, 반응이 오는 경우 → 미래의 신호로 인한 반응

**입력 후**: 입력이 들어간 후 반응이 오는 경우 → 과거의 신호로 인한 반응

그렇다면 Memoryless system는 어떤 경우일까? memoryless의 경우는 그 순간만 반응이 오고 끝나는 system이다. 

추가로 causal system의 경우는 과거와 현재의 입력으로 인해 반응이 오는 경우이다. 즉, 입력을 받는 순간과, 입력 후에 반응하는 과정을 의미하는 것이다. 

### Stable(BIBO Stable) system

이 시스템의 경우는 아래의 그림을 보는 것이 더 편할 것이다. 

![Bibo stable](https://i.imgur.com/QbIQVjS.png)

BIBO Stable system의 기본 조건은 수렴하는 것이다. 

$$|y(t|) = | \int x( \tau ) h ( t - \tau ) d \tau 
| \leq \int |x ( \tau )  h(t - \tau ) | d \tau$$  

$$= \int | x(\tau ) | h( t - \tau )| d\tau$$ (모든 복소수에 대하여)

$$\int |h(t)dt$$가 수렴할 경우, 이를 $B$라 하자.

$$ \int | x(\tau ) | h( t - \tau )| d\tau < B \int |h( t - \tau)| d \tau$$ (수렴)

즉 해당 함수보다 큰 함수가 수렴하므로 $y(t)$가 수렴한다.



