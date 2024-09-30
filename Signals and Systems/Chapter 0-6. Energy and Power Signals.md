# English

### Definition of Energy and Power

First, the total energy can be defined as follows:

$$
\int_{t_1}^{t_2} \left|x(t)\right|^2 dt 
$$

The reason for defining it this way is to maintain consistency with the concept of energy in physics.

Energy, in its basic form, is the physical quantity that arises when work is done on an object. Moreover, energy changes in proportion to the amount of work done.

Since the equation above aligns with the concept in physics, the relationship between power and energy can be expressed through differentiation and integration.

Let's express power using the following formula:

$$
{1\over t_2 - t_1}\int_{t_1}^{t_2} \left|x(t)\right|^2dt
$$

The formula above represents the average power. While it can be expressed in specific intervals, it can also be defined over the entire range as follows:

$$
P = \lim_{T→\infty}{1\over2T}\int_{-T}^{T}\left|x(t)\right|^2dt
$$

$$
E = \lim_{T→\infty}\int_{-T}^{T}\left|x(t)\right|^2dt
$$

Using the equations above, we can now differentiate between energy signals and power signals.

### Energy Signals and Power Signals

What is an energy signal?

An energy signal converges to a non-zero value when the energy is calculated, and its power converges to zero.

What is a power signal?

A power signal diverges in energy, but its power converges to a non-zero value.

This distinction becomes clearer with an example:

$$
x(t) = \begin{cases}1-\left|t\right|&\left|t\right| \leq1 # 0&\text{otherwise}\end{cases}
$$

When this signal is plotted, it appears as follows:

![signal](https://i.imgur.com/pWx2vgP.png)

If we calculate the energy, it converges to a specific value, indicating that this is an energy signal.

Thus, energy signals and power signals can be distinguished this way.

# Korean

### 에너지와 전력의 정의

일단, 전체 에너지의 정의 자체는 다음과 같이 정의할 수 있다. 

$$
\int_{t_1}^{t_2} \left|x(t)\right|^2 dt 
$$

위와 같이 정의한 이유는 물리에서 말하는 에너지와 일맥 상통하게 말하기 위해서이다. 

에너지는 기본적으로 물체에 일을 해줌으로써 발생하는 물리량이다. 또한 일의 양만큼 에너지가 변한다. 

물리학의 개념에 부합하게 위의 공식을 설정했기에, 일률과 에너지의 관계는 미분과 적분의 관계로 표현할 수 있는 것이다.  

이를 이용해서 일률도 공식으로 표현해보자. 

$$
{1\over t_2 - t_1}\int_{t_1}^{t_2} \left|x(t)\right|^2dt
$$

위의 일률은 평균 일률이다. 위와 같이 구간별로 표현하기도 하지만, 전체 구간으로 표현하기도 한다. 각각을 전체 구간으로 표현하면 다음과 같다. 

$$
P = \lim_{T→\infty}{1\over2T}\int_{-T}^{T}\left|x(t)\right|^2dt
$$

$$
E = \lim_{T→\infty}\int_{-T}^{T}\left|x(t)\right|^2dt
$$

이제 위의 식들을 이용해서 에너지 신호와 전력 신호를 구분할 것이다. 

### 에너지 신호와 전력 신호

에너지 신호는?

에너지 값을 계산했을 때, 0이 아닌 값으로 수렴하고, 전력이 0으로 수렴하는 경우이다. 

전력 신호는?

에너지는 발산하고, 전력이 0이 아닌 값으로 수렴하는 경우이다. 

이 부분은 예제를 보면서 생각해야 쉬울 것이다. 

$$
x(t) = \begin{cases}1-\left|t\right|&\left|t\right| \leq1 # 0&\text{otherwise}\end{cases}
$$

위의 신호를 그림으로 표현하면 아래와 같다. 

![signal](https://i.imgur.com/pWx2vgP.png)

에너지를 먼저 구해보면 특정 값으로 수렴하는 것을 알 수 있고 이는 당연하게 에너지 신호이다. 

이렇게 에너지 신호와 전력 신호를 구분해줄 수 있다.

