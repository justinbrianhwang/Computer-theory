# English


$(-1)^x ?$

Let's think about $-1$ on the complex plane.

![Euler](https://i.imgur.com/dcBmgDg.png)

-1 is located at the position shown, which has a magnitude of 1 and is rotated by $\pi$ from the reference point. Thus, the following holds:

$$
-1 = 1 \times e^{\pi j}
$$

Taking the exponent of the above formula:

$$
(-1)^x = (1 \times e^{\pi j})^x
$$

This can be simplified as follows:

$$
e^{\pi j x}
$$

Strictly speaking, there is a mathematical condition that $x$ must be an integer, but let's not worry about the rigorous details for now.

The advantage of representing complex numbers in terms of exponential functions is the simplicity it provides for complex expressions. Consider the following complex numbers:

$$
z_1 =  a_1 + b_1 j
$$

$$
z_2 =  a_2 + b_2 j
$$

$$
z_3 =  a_3 + b_3 j
$$

When expressed this way, multiplying $z_1, ~z_2, ~z_3$ involves very complex operations. However, using Euler's formula, it can be transformed as follows:

$$
z_1 =  a_1 + b_1 j = A_1 e^{j \theta_1}
$$

$$
z_2 =  a_2 + b_2 j = A_2 e^{j \theta_2}
$$

$$
z_3 =  a_3 + b_3 j = A_3 e^{j \theta_3}
$$

Thus, it becomes:

$$
z_1 z_2 z_3 = A_1 A_2 A_3 e^{j(\theta_1 + \theta_2 + \theta_3)}
$$

This simplification is much easier to handle. There are many other advantages to this representation, which we will explore further in due course.

# Korean

$(-1)^x ?$

일단, 복소 평면에서 $-1$을 생각해보자. 

![Euler](https://i.imgur.com/dcBmgDg.png)

-1은 해당위치이며, 이는 크기가 1이고, 기준점에서 $\pi$만큼 회전시킨 부분이므로 다음이 성립한다. 

$$
-1 = 1 \times e^{\pi j}
$$

위의 공식에서 지수를 취해보자. 

$$
(-1)^x = (1 \times e^{\pi j})^x
$$

이렇게 수정이 가능하며, 다음과 같이 정리 된다. 

$$
e^{\pi j x}
$$

물론 엄밀하게 수학적으로는 $x$가 정수여야 한다는 조건이 있지만, 엄밀한 부분에 대해서는 일단은 생각하지 말자. 

사실 복소수라는 내용을 복잡한 식에서 단순하게 지수함수의 형태로 표현할 수 있다는 장점이 있기에 사용하는 것이다. 아래의 식들을 보자 

$$
z_1 =  a_1 + b_1 j
$$

$$
z_2 =  a_2 + b_2 j
$$

$$
z_3 =  a_3 + b_3 j
$$

위와 같이 표현한 경우, $z_1, ~z_2 , ~z_3$ 를 곱할 경우 매우 복잡한 연산을 해야 한다. 그렇다면 이를 오일러 공식으로 변환시키면 어떻게 나올까? 

$$
z_1 =  a_1 + b_1 j = A_1 e^{j \theta_1}
$$

$$
z_2 =  a_2 + b_2 j = A_2 e^{j \theta_2}
$$

$$
z_3 =  a_3 + b_3 j = A_3 e^{j \theta_3}
$$

이렇게 표현이 가능하며, 

$$
z_1 z_2 z_3 = A_1 A_2 A_3 e^{j(\theta_1 + \theta_2+ \theta_3)}
$$

위와 같이 단순한 연산이 가능해진다. 이 외에도 너 많은 편리함을 가진다는 장점이 있지만 그 외적인 것은 차차 다루도록 할 것이다.

