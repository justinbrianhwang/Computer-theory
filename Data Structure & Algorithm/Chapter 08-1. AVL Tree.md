# English

# AVL Tree

- What is a BST?
- Disadvantages of BST
- How to overcome BST's disadvantages
- What is an AVL Tree?
- AVL Tree Rotations and Construction
- Cases with Many Children

The above topics will be discussed.

### What is a BST?

A tree like the one below is called a Binary Search Tree (BST).

![BST](https://i.imgur.com/S5mJN5e.png)

This type of tree is useful for searching. For example, the left child of a parent node holds a value smaller than the parent, and the right child holds a value larger than the parent. This property makes it efficient for searching.

Let's assume we want to find the value 30.

![BST2](https://i.imgur.com/AiVPoa6.png)

![BST3](https://i.imgur.com/BZys3kO.png)

![BST4](https://i.imgur.com/zvcDzkT.png)

The search follows this process. If the node is not found, it traverses until it reaches the end and returns a NULL value.

The number of searches in a BST depends on its height, and can be represented as:

$$
\begin{cases}
\text{min} = \log n \\ 
\text{max} = n
\end{cases}
$$

What are the disadvantages of this BST?

### Disadvantages of BST

The structure of a BST can be inefficient depending on the order in which the tree is built. Let’s build a tree with the following sequence:

30, 40, 10, 50, 20, 5, 35

Let’s look at this process:

![AVL5](https://i.imgur.com/GmnzTLp.png)

In this case, efficient searching is possible.

Now, let’s build the tree with the following sequence:

50, 40, 35, 30, 20, 10, 5

Let’s observe this process:

![AVL6](https://i.imgur.com/I5gEykT.png)

The tree in the image above has a height of 7.

The tree with a smaller height is more efficient for searching, requiring a maximum of 3 searches, whereas the taller tree may require up to 7 searches. The major disadvantage of a BST is that its efficiency can vary greatly depending on the insertion order.

Now let’s see how to overcome the disadvantages of a BST.

### Overcoming BST's Disadvantages

To simplify the explanation, let’s use three nodes: 10, 20, and 30. If we insert the nodes in the order 30, 20, 10, the tree will look like this:

![BST](https://i.imgur.com/Crletmd.png)

Of course, this is how it would be structured. There are $3!$ or $6$ different ways to arrange these three nodes, and the most efficient arrangement is:

![BST2](https://i.imgur.com/KUGzYE6.png)

The process of transforming the tree from the top image to the bottom one is how we overcome the disadvantages of a BST. Our goal is to create a tree with a lower height. The process involves transforming the tree to the following form:

![BST3](https://i.imgur.com/w9D5ZGO.png)

In the end, our task is to minimize the tree’s height. This is where the AVL tree comes into play!

### What is an AVL Tree?

First, let’s define the term "balance factor". The balance factor is defined as follows:

$$
\text{balance factor} = \text{height of left subtree} - \text{height of right subtree}
$$

In other words, it’s the difference between the left and right subtree heights. The balance factor, abbreviated as $\text{bf}$, is calculated as $\text{bf} = \text{hl} - \text{hr} = \{-1, 0, 1\}$.

If the balance factor is not $-1$, $0$, or $1$, the tree is considered unbalanced. If it is within this range, the tree is balanced. Our goal is to maintain a balanced tree.

Let’s look at some examples. Below is an illustration:

![AVL](https://i.imgur.com/urTdW31.png)

The tree above maintains a proper balance factor, making it a balanced tree. However, the tree below is not balanced.

Now that we have distinguished between balanced and unbalanced trees, let’s look at the process of constructing an AVL tree.

### AVL Tree Construction

It’s best to explain this process with diagrams.

![avl](https://i.imgur.com/0lS67kq.png)

In the diagram above, the balance factor is 2, which is called an LL-imbalance. The rotation required here is called an LL-Rotation.

Next is the case of an LR-imbalance, as shown below:

![avl2](https://i.imgur.com/FRcBgpi.png)

In this case, both left and right rotations are required to restore balance. This is called an LR-Rotation.

The other rotations, RR-Rotation and RL-Rotation, can be explored by the reader.

### AVL Tree with Many Children

So far, we’ve only looked at cases where the tree is relatively simple. Now, let’s consider the case where the tree has many children. Although the logic remains the same, there are some subtle differences in detail.

Again, this is best illustrated with a diagram.

![avl](https://i.imgur.com/8k2ak17.png)

As shown in the diagram, when an AVL tree has many children, it is important to determine which values are smaller or larger than a given value and perform LL, LR, RL, or RR rotations accordingly.

# Korean

# AVL Tree

- BST란?
- BST의 단점
- BST의 단점 개선 방법
- AVL Tree란?
- AVL Tree의 회전과 제작
- 자식의 수가 많은 경우

위와 같은 내용을 다룰 것이다.

### BST란 무엇일까?

아래와 같은 형태의 tree를 BST라 한다. 

![BST](https://i.imgur.com/S5mJN5e.png)

이런 트리는 검색에 유용한 tree이다. 예를 들어, 부모의 왼쪽 자식은 부모보다 작은 값이, 부모의 오른쪽은 부모보다 큰 값이 위치하게 된다. 이러한 특성으로 인해 검색에 유용한 것이다. 

예를 들어 30을 찾는다고 가정을 해보자. 

![BST2](https://i.imgur.com/AiVPoa6.png)

![BST3](https://i.imgur.com/BZys3kO.png)

![BST4](https://i.imgur.com/zvcDzkT.png)

이런 과정을 거쳐 찾는 것이다. 노드가 없을 경우에 끝까지 확인하고 NULL 값으로 반환하는 방식인 것이다. 

이러한 BST의 검색 횟수는 높이에 의존하는데, 

$$
\begin{cases}
\text{min} = \log n \\ 
\text{max} = n
\end{cases}
$$

와 같이 검색 횟수를 확인할 수 있다. 

### BST의 단점

BST는 순서에 따라 Tree의 구성이 비효율적일 수도 있다는 것이다. 먼저 다음과 같은 순서로 트리를 구성해보자. 

30, 40, 10, 50, 20, 5, 35

이 과정을 보도록 하자. 

![AVL5](https://i.imgur.com/GmnzTLp.png)

이렇게 설계된다. 즉 이 경우는 효율적인 탐색이 가능해진다. 

이와 달리 다음과 같은 순서로 트리를 구성해보자. 

50, 40, 35, 30, 20, 10, 5

이 과정을 보자. 

![AVL6](https://i.imgur.com/I5gEykT.png)

위의 트리는 높이가 7인 트리이다. 

위와 아래 중 높이가 작은 위 트리는 검색에 유용하며, 최대 3번의 검색을 진행하나, 아래 트리는 최대 7번 검색을 진행하는 것이다. BST 구성 시, 순서에 따라 효율적일 수도, 비효율적일 수도 있다는 것이 BST의 큰 단점인 것이다.

### BST 단점 극복

단순한 구조 설명을 위해 3개의 노드로 설명하도록 할 것이다. 10, 20, 30이라고 하자. 순서를 다르게 줄 것인데, 30, 20, 10 순서로 준다고 해보자. 

![BST](https://i.imgur.com/Crletmd.png)

당연히 이렇게 구성이 될 것이다. 이와 같이 순서를 다르게 한 경우 총 $3!$가지 즉 $6$가지가 될 것이다. 그 중 가장 효율적인 구성은 아래와 같을 것이다. 

![BST2](https://i.imgur.com/KUGzYE6.png)

즉 위의 그림에서 아래 그림으로 만들어 주는 과정이 바로 단점 극복이 될 것이다. 우리가 원하는 바는 높이가 낮은 트리를 만드는 것이다. 일단 형태만을 보면 각각 다음과 같이 변형 시켜야 한다. 

![BST3](https://i.imgur.com/w9D5ZGO.png)

결국 우리가 해줘야 할 작업은 이런 것이다. 어떻게 높이를 최소화시킬 수 있을까? 이 고민으로부터 AVL 트리가 나온 것이다! 

### AVL tree가 무엇일까?

먼저 용어부터 정리하고 가자. 바로 balance factor이다. 이 용어의 정의는 아래와 같다. 

$$
\text{balance factor} = \text{height of left subtree} - \text{height of right subtree}
$$

즉, 왼쪽 높이 - 오른쪽 높이이다. 이를 줄여, $\text{bf}$로 표현하기도 한다. 즉, $\text{bf} = \text{hl} - \text{hr} = \{-1, 0, 1\}$

bf의 값이 위의 $-1, 0, 1$이 아니라면 이를 불균형 트리, 맞다면 균형 트리라 하며, 우리의 지향점은 균형 트리인 것이다. 

### AVL Tree 제작

이는 그림을 통해 보는 것이 좋을 것이다. 

![avl](https://i.imgur.com/0lS67kq.png)

위는 bf가 2이다. 즉 이러한 경우를 LL-imbalance라 한다. 또한 이러한 회전을 LL-Rotation이라 한다. 

다음은 LL-Rotation을 다룬 것이다. 그렇다면 다른 경우는 뭐가 있을까? 아래의 사진을 보자. 

![avl2](https://i.imgur.com/FRcBgpi.png)

이는 각각 왼쪽 회전과 오른쪽 회전을 진행해야 balance를 맞출 수 있다. 이러한 상황을 LR-imbalance라 하며, 이러한 회전을 LR-Rotation이라 한다. 

### AVL Tree의 자식이 많은 경우

지금까지는 단순하게 채우는 경우만을 봐왔다. 이번에는 자식이 많은 트리의 경우를 확인해보도록 하자. 논리 구조 자체는 동일하나, 약간의 디테일 차이가 존재한다. 

이 또한 그림으로 보는 것이 좋을 것이다. 

![avl](https://i.imgur.com/8k2ak17.png)

위의 그림과 같이 AVL 자식이 많은 경우, 해당 자식들이 어떤 값보다 작고, 어떤 값보다 큰지를 결정하여 LL회전, LR회전, RL회전, RR회전을 진행해야 하는 것이다.

