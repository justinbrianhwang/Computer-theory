# English

### Example of Euler's Formula → Finding Magnitude and Angle

Any form of complex function can be expressed in the form \(Ae^{j \theta}\). 

To find \(\theta\), we use the \(\arctan\) function. Let's consider a point on the complex plane, denoted as \((a, ~b)\). The point can be illustrated as follows:

![euler](https://i.imgur.com/aNgVZlo.png)

To find the angle \(\theta\) from the real axis to the point, we can use a supplementary line, as shown in the diagram below:

![euler2](https://i.imgur.com/NtrxoL0.png)

From the diagram, the angle is given by:

$$
\theta = \arctan\left(\frac{b}{a}\right)
$$

The magnitude \(A\) is the distance from the origin to the point, given by \(\sqrt{a^2 + b^2}\).

Now, let's express the function \(1+e^{j5t}\) in the form \(Ae^{j \theta}\).

First, express \(e^{j5t}\) as a sum of \(\sin\) and \(\cos\): \(e^{j5t} = \cos(5t) + j \sin(5t)\). So, \(1 + \cos(5t) + j \sin(5t)\) can be separated into:

- Real part: \(1+\cos(5t)\)
- Imaginary part: \(\sin(5t)\)

The angle is calculated as \(\theta = \arctan\left(\frac{\sin(5t)}{1 + \cos(5t)}\right)\), and the magnitude is \(A = \sqrt{(1+\cos(5t))^2 + (\sin(5t))^2}\).

Thus, the function \(1 + e^{j5t}\) can be expressed in the form \(Ae^{j \theta}\) as follows:

$$
1+e^{j5t} = \sqrt{(1+ \cos(5t))^2 + (\sin(5t))^2} \cdot e^{j \arctan\left(\frac{\sin(5t)}{1 + \cos(5t)}\right)}
$$

Using this method, you can express given functions using Euler's approach.


# Korean


### 오일러 공식 예제 → 크기와 각도 구하기

어떠한 형태의 함수들도 우리는 \(Ae^{j \theta}\)의 형태로 표현할 수 있다.

이때, 우리는 \(\theta\)를 알아봐야 하는데, 이는 \(\arctan\)을 이용해서 구해야 한다. 임의의 복소 평면에서의 점을 생각해보자. 이때 점은 \((a, ~b)\)라 하자. 그렇다면 그림은 다음과 같이 그려질 수 있다.

![euler](https://i.imgur.com/aNgVZlo.png)

이 점에서 실수 축으로부터의 각도인 \(\theta\)를 구하기 위해, 보조선을 이용해서 표현하면 아래의 그림과 같다.

![euler2](https://i.imgur.com/NtrxoL0.png)

다음 그림에서 각도는 아래와 같다.

$$
\theta = \arctan\left(\frac{b}{a}\right)
$$

또한 \(A\)는 해당 점에서 원점까지의 거리인 \(\sqrt{a^2 + b^2}\)이다.

이제 실제 함수 중 \(1+e^{j5t}\)를 \(Ae^{j \theta}\)의 형태로 표시하자.

먼저, \(e^{j5t}\)를 \(\sin\)과 \(\cos\)의 합으로 표현하면, \(\cos(5t) + j \sin(5t)\)이다. 즉, \(1 + \cos(5t) + j \sin(5t)\)이다.

실수 부분: \(1+\cos(5t)\)

허수 부분: \(\sin(5t)\)

이렇게 두 부분으로 나누어 생각할 수 있고,

각을 구하면 \(\theta = \arctan\left(\frac{\sin(5t)}{1 + \cos(5t)}\right)\)이고, 크기는 \(A = \sqrt{(1+\cos(5t))^2 + (\sin(5t))^2}\)이다.

구할 부분을 전부 구했으므로 주어진 함수인 \(1 + e^{j5t}\)를 \(Ae^{j \theta}\)의 형태로 표현하면 다음과 같다.

$$
1+e^{j5t} = \sqrt{(1+ \cos(5t))^2 + (\sin(5t))^2} \cdot e^{j \arctan\left(\frac{\sin(5t)}{1 + \cos(5t)}\right)}
$$

앞으로 주어진 함수들을 오일러 방법으로 표현할 수 있을 것이다.

