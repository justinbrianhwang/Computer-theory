# English

### $m$-way Tree

Before diving into B-Trees, we first need to understand the concept of an $m$-way Tree!

We all know that the Binary Search Tree (BST) is advantageous for searching. A BST looks like the following:

![BST](https://i.imgur.com/S5mJN5e.png)

However, the limitation of a BST is that it has only one key per node and at most two children. Although the AVL Tree we discussed earlier is also a type of BST, we won't go into detail about it here!

Our goal now is to increase the number of keys and children. This leads to structures like the following:

![mway Tree](https://i.imgur.com/cvMAQZ9.png)

The tree above has 2 key values and 3 children! Like a BST, this structure is efficient for searching. Here’s the basic idea:

In an $m$-way tree, the number of children is $m$, and the number of keys is $m - 1$. Let's take a closer look at the structure of a node in an $m$-way tree.

![mway Tree2](https://i.imgur.com/tVKL4gA.png)

This is a node in a 5-way tree. It has 5 child pointers and 4 keys.

While an $m$-way tree can store much more information and seems more efficient for searching, it has significant drawbacks, which is why it’s not commonly used.

### Drawbacks of $m$-way Trees

Consider the following scenario:

The key values are 10, 20, 30, etc.

Different users will insert these values in various ways. Since there is no strict rule for the structure, the number of layers is not limited. To illustrate what this means, take a look at the image below:

![back draw](https://i.imgur.com/P8IFrwf.png)

On the left, we see an inefficient insertion, while on the right, the insertion is efficient. Since there is no guiding structure, the tree on the left becomes less efficient for searching, while the tree on the right remains highly efficient.

### B-Tree

A B-Tree solves these issues by providing rules and guidelines!

Let's outline the rules for B-Trees:

1. Each node must be filled with at least $\lceil {m\over2} \rceil$ keys.
2. The root node can have fewer than two children.
3. All leaves are at the same level.
4. The tree maintains balance by rebalancing through upward structures during insertion and deletion.




# Korean


## B-Tree

### $m$-way Tree

우리가 B-Tree를 보기 전에, 먼저 봐야 할 내용이 있다. 바로 $m$-way Tree이다!

기존에 우리가 배웠던 BST는 검색에 유리한 트리임은 누구나 알고 있을 것이다. BST의 모양은 다음과 같이 생긴 것이다.

![BST](https://i.imgur.com/S5mJN5e.png)

다만 BST의 한계는 key가 1개, 자식의 수가 2개라는 점이다. 물론 앞장에서 다룬 AVL 트리 또한 BST의 종류 중 하나이니, 굳이 언급하지는 않을 것이다!

즉, 우리의 목적은 자식의 수를 늘리고, key를 늘리는 것이다. 즉, 아래와 같은 형태로 만드는 것이다.

![mway Tree](https://i.imgur.com/cvMAQZ9.png)

위의 트리는 2개의 key 값을 갖고, 3개의 자식을 갖는 형태이다! 이 또한 BST처럼 검색에 유리한 트리이다. 여기서 우리는 정보를 살펴볼 수 있는데

$m$-way 트리라 할 때, 자식의 수는 $m$, key의 수는 $m - 1$이다. $m$-way 트리의 노드 형태를 단순하게 살펴보도록 하자.

![mway Tree2](https://i.imgur.com/tVKL4gA.png)

위의 트리는 $5$-way 트리의 노드 구조이다. 자식을 가리키는 주소 값이 5개이며, key 값은 4개임을 확인할 수 있다.

사실 BST보다 훨씬 많은 정보를 담을 수 있고, 더 효율적으로 검색이 가능해 보이지만 아주 큰 단점이 존재하기에 $m$-way Tree를 많이 사용하지 않는 것이다.

### $m$-way Tree 단점

단순하게 아래의 상황을 생각해보자.

key 값은 10, 20, 30, ..이다.

사용자마다 넣는 방법은 다르게 적용할 것이다. 즉, 규칙이 적용되지 않았기에 layer 수가 제한되지 않는다. 이 말이 무슨 의미냐면, 아래의 그림을 보면 된다.

![back draw](https://i.imgur.com/P8IFrwf.png)

왼쪽의 경우 비효율적으로 삽입한 경우고, 오른쪽의 경우 효율적으로 삽입한 것이다. 이는 규칙이 없는 트리이기에, 왼쪽의 경우는 검색에 오히려 불리하고 오른쪽은 매우 효율적인 것이다.

### B Tree

rule과 guide line을 제공해주는 tree가 바로 B tree이다!

먼저, rule부터 정리해보자.

1. $\lceil {m\over2} \rceil$는 반드시 노드마다 채워져 있어야 한다.
2. Root는 두 자식보다 적게 가질 수 있다.
3. 모든 leaf는 같은 레벨이다.
4. 항상 상향구조인데, 삽입 삭제 시 균형을 맞추기 위해 상향을 한다는 의미이다.




