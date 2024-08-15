# English

## Basic Assumptions in Circuit Theory

### Relationship Between Electromagnetics and Circuit Theory

Electromagnetics, typically covered in general physics or electromagnetics courses, deals with electric fields, magnetic fields, and electromagnetic waves using vector analysis. The variables in electromagnetics include spatial and time variables, resulting in a complex system involving four variables. Circuit theory, on the other hand, simplifies this by analyzing electromagnetics algebraically, turning vector equations into systems of linear equations. Essentially, it transforms the vector analysis into an algebraic approach.

The following diagram illustrates this concept:

![circuit](https://i.imgur.com/HUIn31v.png)

To transition from electromagnetics to circuit theory, three fundamental assumptions must be made.

### Three Assumptions for Applying Circuit Theory

1. **Electrical effects propagate instantaneously within a system.**

    Consider the physical size of a circuit, denoted as $x$. If the wavelength of the electromagnetic wave is more than ten times greater than $x$, then $x$ becomes negligible. This allows us to ignore the spatial variables $x$, $y$, and $z$, leaving only the time variable. Originally, an electromagnetic wave is expressed as:

$$
    y(x,~ t) = A\sin 2 \pi \left( \frac{t}{T} - \frac{x}{\lambda} \right)
$$

where $T$ is the period, and $\lambda$ is the wavelength. If $\lambda \gg x$, the amplitude function simplifies to:

$$
    y(t) = A \sin \frac{2 \pi t}{T}
$$

A system where $\lambda \gg x$ is referred to as a lumped parameter system. 

The assumption of instantaneous propagation means, for example, that in a circuit connecting the Earth and the Moon, an event at one end is felt immediately at the other end. Consider the scenario where a switch on Earth is flipped at $t = 0$, causing a voltage change at a resistor on the Moon. The voltage change at the resistor on Earth happens simultaneously with the one on the Moon:

![earth moon](https://i.imgur.com/iBDy0Ws.png)

![earth moon2](https://i.imgur.com/9Qbihz7.png)

2. **The net charge stored in any component within the system is always zero.**

For example, in a capacitor, while it may appear that a specific charge like $3C$ is stored, the net charge across the capacitor plates is zero since the charges are distributed across the positive and negative plates.

3. **There is no magnetic coupling between components within the system.**

    The diagram below clarifies this assumption:

    ![system](https://i.imgur.com/4uc9rRV.png)

    While magnetic fields may interact, circuit theory assumes that they do not influence each other.

## Key Units and Exponential Notation

### Key Units

1. Frequency, Hertz (Hz), $\text{s}^{-1}$
2. Force, Newton (N), $\text{kg} \cdot \text{m/} \text{s}^2$
3. Energy or Work, Joule (J), $\text{N} \cdot \text{m}$
4. Power, Watt (W), $\text{J/s}$
5. Charge, Coulomb ($\text{C}$), $\text{A} \cdot \text{s}$
6. Voltage, Volt ($\text{V}$), $\text{J/C}$
7. Resistance, Ohm ($\Omega$), $\text{V/A}$
8. Conductance, Siemens ($\text{S}$), $\text{A/V}$
9. Capacitance, Farad ($\text{F}$), $\text{C/V}$
10. Magnetic Flux, Weber ($\text{Wb}$), $\text{V} \cdot \text{s}$
11. Inductance, Henry ($\text{H}$), $\text{Wb/A}$

### Exponential Notation

1. pico, $10^{-12}$, $\text{p}$
2. nano, $10^{-9}$, $\text{n}$
3. micro, $10^{-6}$, $\mu$
4. milli, $10^{-3}$, $\text{m}$
5. kilo, $10^{3}$, $\text{k}$
6. mega, $10^{6}$, $\text{M}$
7. giga, $10^{9}$, $\text{G}$
8. tera, $10^{12}$, $\text{T}$

→ Memorize all the key units and exponential notations.

## Definitions and Representations of Voltage, Current, and Power

### Current

**Definition**

Current is defined as the rate of change of charge $q$ with respect to time. The unit is the Ampere [A].

$$
i = \frac{dq}{dt}
$$

**Representation**

When current $i$ flows from terminal $a$ to terminal $b$ in a component, it can be expressed in two ways:

1. Current $i$ flows from $a$ to $b$.
2. Current $-i$ flows from $b$ to $a$.

Although the idea of negative current might seem odd, it is used for mathematical convenience.

![current](https://i.imgur.com/K5lVAdD.png)

### Voltage

**Definition**

Voltage is defined as the rate of change of energy $w$ required to move a charge $q$ from point $a$ to point $b$ in an electric field, with the unit being Volts [V].

$$
v = \frac{dw}{dq}
$$

**Representation**

If terminal $a$ has a higher voltage than terminal $b$ by $v$, this can be expressed in two ways:

1. Terminal $a$ is $v$ volts higher than terminal $b$.
2. Terminal $b$ is $-v$ volts higher than terminal $a$.

![voltage](https://i.imgur.com/V0jcQbt.png)

The energy being referred to can be understood better with the following diagram:

![voltage2](https://i.imgur.com/KB6GkYY.png)

When moving from point $b$ to point $a$, the voltage can be calculated as $v = \frac{dw}{dq}$.

### Power

Power is defined as $p = \frac{dw}{dt}$. This can be further simplified to:

$$
p = \frac{dw}{dt} = \frac{dw}{dq} \times \frac{dq}{dt} = v \times i = vi[\text{W}]
$$

This is the basic definition to be aware of.

### Voltage Drop and Voltage Rise

- **Voltage Drop:** When moving within a circuit element from the terminal with a higher voltage (+) to the terminal with a lower voltage (-).
- **Voltage Rise:** When moving within a circuit element from the terminal with a lower voltage (-) to the terminal with a higher voltage (+).

## Conventional Current

### Understanding of Current Before the Discovery of Electrons

It was believed that positive charges flowed from the positive terminal to the negative terminal.

![Conventional](https://i.imgur.com/dUJ4LI4.png)

### Understanding of Current After the Discovery of Electrons

It became understood that negative charges (electrons) flow from the negative terminal to the positive terminal.

![Conventional2](https://i.imgur.com/Z86WHnn.png)

### There Is No Difference in the Concept of Current

For convenience, circuit theory typically assumes that positive charges flow from the positive terminal to the negative terminal, as in the original concept.

## Passive Sign Convention

### Voltage Polarity and Current Direction in a Component

(1) There are four ways to define the voltage polarity and current direction in a component:

![passive sign convention](https://i.imgur.com/u1OUr6o.png)

(2) In the first and fourth diagrams, current flows into the positive terminal of the component and out of the negative terminal, meaning the current direction is the same as the voltage drop direction.

(3) The first and fourth diagrams satisfy the passive sign convention.

### Power and Passive Sign Convention in a Component

(1) When calculating power $p = vi$, it must be determined whether the component is absorbing or supplying power.

(2) If the passive sign convention is satisfied, $p = vi$ represents the power absorbed by the component.

(3) If the passive sign convention is violated, $p = vi$ represents the power supplied by the component to the outside.

### Voltage-Current Relations in RLC Components and the Passive Sign Convention

(1) The following voltage-current relations in $\text{RLC}$ components are valid under the passive sign convention:

$$
v = Ri, \quad v = L \frac{di}{dt}, \quad i = C \frac{dv}{dt}
$$

(2) Although the voltage and current in a component can be defined arbitrarily, when writing the voltage-current relation, the voltage polarity or current direction must be adjusted to satisfy the passive sign convention.

![current](https://i.imgur.com/uVk3lBW.png)




# Korean

## 회로이론의 기본가정

### 전자기학과 회로이론의 관계

주로 일반물리학이나, 전자기학에서 배우는 전자기학은 전기장, 자기장, 전자기파 등을 벡터 해석을 이용해서 다룬다. 이때 전자기학에 다루는 변수는 위치변수, 시간변수를 다루기에, 총 4개의 변수를 다루는 사실상 복잡한 변수이다. 이러한 전자기학을 대수적으로 해석하는 것이 바로 회로이론이다. 벡터들을 연립방정식으로 풀이하는 방법이다. 즉 벡터해석에서, 대수적 방법으로 바꾸는 것이라 생각하면 쉽다.

다음 그림을 보면 쉽게 이해할 수 있을 것이다.

![circuit](https://i.imgur.com/HUIn31v.png)

그렇다면 전자기학에서 회로이론으로 적용을 시키기 위한 세 가지 가정을 알아보자.

### 회로이론이 적용되기 위한 세 가지 가정

1. **전기 효과는 하나의 시스템 내에서 순간적으로 전파된다.**

    회로의 물리적 크기를 $x$라 하자. 이때 전자기파의 파장이 10배 이상으로 크다고 하면, $x$는 무시가능한 크기가 된다. 이렇기에 벡터들의 공간인 $x,~ y,~ z$를 무시할 수 있게 되고, 시간만 남게 된다. 즉 원래 전자기파는 다음과 같다.

$$
    y(x,~ t) = A\sin 2 \pi \left( \frac{t}{T} - \frac{x}{\lambda} \right)
$$

이며, $T$는 주기, $\lambda$는 파장을 의미하는 것이다. 하지만, 위에서 언급한 대로 $\lambda \gg x$이면 진폭함수는 다음과 같다.

$$
    y(t) = A \sin \frac{2 \pi t}{T}
$$

이때,  $\lambda \gg x$가 성립하는 시스템을 집중 정수계라 한다.

그렇다면 위에서 언급한 순간적으로 전파된다는 말은 무슨 의미일까? 예를 들어 지구와 달을 연결한 긴 회로가 있다고 가정하자.

그렇다면 아래의 그림과 같은 상황이 발생한다.

![earth moon](https://i.imgur.com/iBDy0Ws.png)

초기 상황은 다음과 같다. $t=0$에서 스위치를 누르는 것이다. 달에 위치한 저항은 현재는 $0V$이다. 하지만 $t= 0$ 에서 스위치를 누른 상황을 생각해보자.

![earth moon2](https://i.imgur.com/9Qbihz7.png)

   누르는 동시에 달에 있는 저항과 스위치 옆에 바로 있는 저항에 동시에 $2V$로 전압이 잡히게 되는 것이다.

2. **시스템 내의 각 소자의 저장 전하량은 항상 0이다.**

    축전기 같은 소자를 생각하면 $3C$과 같은 특정한 전력이 잡혀있음을 알 수 있다. 이를 보면 저장 전하량이 $0$이 아닌 것 같다는 생각이 들겠지만, 이는 전하량이 +- 극판에 각각 분포되어 있어서 알짜 전하량을 구하면 여전히 $0$이다.

3. **시스템 내의 각 소자들 간의 자기적 결합은 없다.**

    이 부분은 그림부터 보는 것이 더 효율적으로 정리할 수 있을 것이다.

    ![system](https://i.imgur.com/4uc9rRV.png)

    자기장이 서로 영향을 받지만, 회로 이론에서는 그렇지 않음을 가정하는 것이다.

## 주요 단위 및 십의 거듭 제곱 표시

### 주요 단위

1. 주파수, 헤르츠(Hz), $\text{s}^{-1}$
2. 힘, 뉴턴(N), $\text{kg} \cdot \text{m/} \text{s}^2$
3. 에너지 또는 일, 줄(J), $\text{N} \cdot \text{m}$
4. 전력, 와트(W), $\text{J/s}$
5. 전하, 쿨롱($\text{C}$), $\text{A} \cdot \text{s}$
6. 전위, 볼트($\text{V}$), $\text{J/C}$
7. 저항, 옴($\Omega$), $\text{V/A}$
8. 컨덕턴스(전도도), 지멘스($\text{S}$), $\text{A/V}$
9. 커패시턴스(전기용량), 패럿($\text{F}$), $\text{C/V}$
10. 자속, 웨버($\text{Wb}$), $\text{V} \cdot \text{s}$
11. 인덕턴스(유도계수), 헨리($\text{H}$), $\text{Wb/A}$

### 십의 거듭제곱표시

1. pico, $10^{-12}$, $\text{p}$
2. nano, $10^{-9}$, $\text{n}$
3. micro, $10^{-6}$, $\mu$
4. milli, $10^{-3}$, $\text{m}$
5. kilo, $10^{3}$, $\text{k}$
6. mega, $10^{6}$, $\text{M}$
7. giga, $10^{9}$, $\text{G}$
8. tera, $10^{12}$, $\text{T}$

→ 주요 단위와 십의 거듭제곱 표시는 전부 외우자..

## 전압, 전류, 전력의 정의 및 표현법

### 전류

**정의**

전하량 $q$의 시간에 따른 변화율로 정의한다. 단위는 암페어[A]를 사용한다.

$$
i = \frac{dq}{dt}
$$

**표현방법**

소자의 a 단자에서 b 단자로 전류 $i$가 흐르는 경우 표현 방법은 다음 두 가지가 있다.

1. a에서 b로 전류 $i$가 흐른다.
2. b에서 a로 전류 $-i$가 흐른다.

사실 음수의 전류로 흐름을 표현하는 방식은 와닿지는 않을 것이다. 수학적으로 설명하기 위해 음수를 표현한 것이다. 말 자체는 의미가 없을 수 있지만 수학적 설명으로는 의미가 있기에 남긴다는 것이다.

![current](https://i.imgur.com/K5lVAdD.png)

이렇게 생각하면 된다.

### 전압

**정의**

전기장 속의 두 점 a, b가 있을 때 전하량 $q$의 전하를 점 a에서 b로 이동시키는데 필요한 에너지 $w$의 전하량 $q$에 따른 변화율로 정의하며 단위는 볼트[V]를 사용한다.

$$
v = \frac{dw}{dq}
$$

**표현방법**

소자의 a 단자가 b단자보다 전압 $v$가 높은 경우 표현 방법은 다음 두 가지가 있다.

1. 단자 a가 b보다 $v$만큼 전압이 높다.
2. 단자 b가 a보다 $-v$만큼 전압이 높다.

![voltage](https://i.imgur.com/V0jcQbt.png)

구체적인 에너지가 무엇일까? 정확한 에너지를 그림을 통해 확인해보자.

![voltage2](https://i.imgur.com/KB6GkYY.png)

지점 b에서 지점 a로 갈 때 에너지를 $w = f(q)$라 생각하고, 이때 전압은 위에서 구하는 방식대로 구하면 된다. $v = \frac{dw}{dq}$라 할 수 있다.

### 전력

$p = \frac{dw}{dt}$로 정의한다. 이를 잘 정리하면 다음과 같다.

$$
p = \frac{dw}{dt } = \frac{dw}{dq } \times \frac{dq}{dt} = v \times i = vi[\text{W}]
$$

일단은 이렇게 정의됨을 알아야 한다.

### 전압강화와 전압 상승

- **전압강화:** 회로 내에 어느 소자의 전압극성이 +인 단자에서 -인 단자로 이동하는 경우(전압이 낮아지는 경우)
- **전압 상승:** 회로 내에 어느 소자의 전압 극성이 -인 단자에서 +인 단자로 이동하는 경우(전압이 높아지는 경우)

## 관습적인 전류

### 전자가 발견되기 전 전류에 대한 생각

양극에서 음극으로 양의 전하가 흐르는 것으로 생각했다.

![Conventional](https://i.imgur.com/dUJ4LI4.png)

### 전자가 발견된 후 전류에 대한 생각

음극에서 양극으로 음의 전하가 흐르는 것으로 생각이 되었다.

![Conventional2](https://i.imgur.com/Z86WHnn.png)

### 전류에 관해 어느 경우로 생각하여도 차이가 없다.

기존의 생각과 같이 양극에서 음극으로 양의 전하가 흐른다고 생각하는 것이 편리하므로 회로 이론에서는 1과 같이 생각한다.

## 수동 부호 규정

### 소자의 전압 극성, 전류의 방향

1. 어느 소자에 전압 극성 및 전류 방향을 부여하는 방법은 아래의 4가지의 방법이 존재한다.

![passive sign convention](https://i.imgur.com/u1OUr6o.png)

2. 위의 그림에서 첫 번째와 네 번째는 전류의 소자의 +극으로 흘러 들어가 -극으로 흘러 나온다. 즉, 전류의 방향이 소자의 전압강하방향과 동일한 것이다.

3. 첫 번째와 네 번째는 수동부호규정을 만족하는 것이다.

### 소자의 전력과 수동 부호 규정

1. 전력은 $p = vi$의 계산과 함께 그것이 소자의 흡수 전력인지 공급 전력인지 밝혀야 한다.

2. 수동 부호 규정을 만족하는 경우 $p = vi$는 그 소자가 흡수하는 전력이다.

3. 수동 부호 규정에 어긋나는 경우 $p = vi$는 그 소자가 외부로 공급하는 전력이다.

### RLC 소자의 전압, 전류 관계식과 수동 부호 규정

1. 아래의 $\text{RLC}$ 소자 전압, 전류 관계식은 수동 부호 규정 하에서 성립하는 것이다.

$$
v = Ri, \quad v = L \frac{di}{dt}, \quad i = C \frac{dv}{dt}
$$

2. 소자에 걸리는 전압, 흐르는 전류는 임의로 잡을 수 있으나, 그 전압, 전류 관계식을 쓸 때에는 수동 부호 규정을 만족하도록 전압 극성 또는 전류 방향을 보정해준다.

![current](https://i.imgur.com/uVk3lBW.png)




