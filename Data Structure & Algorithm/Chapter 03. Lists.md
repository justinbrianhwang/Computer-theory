# Enlgish

## List

A list is a data structure that stores elements in a sequential order, similar to the lists we commonly use. There are two main ways to implement a list:

- Array
- Linked List

Let's explore each method.

### Array List

An array is a data structure that allocates memory sequentially, making it straightforward to understand as a linear structure. However, an algorithm is necessary to maintain the order. Consider an array list configured as follows:

![array](https://i.imgur.com/fBHK3j8.png)

Inserting an element at the second position involves the following process:

![array move](https://i.imgur.com/Kw4by1r.png)

Similarly, for deletion:

![array remove](https://i.imgur.com/jNSazoo.png)

Deleting the second element:

![array remove2](https://i.imgur.com/WJfzjnO.png)

You can view the C file I wrote for the array list implementation by clicking the following link. These functions are my creations, though there may be similar code by others. If you use my code, please credit the source.

[]()

### Linked List

Unlike array lists, linked lists have no size limitations. Once an array's size is set, it can't be changed, but theoretically, a linked list can grow indefinitely.

**Structure of a Linked List**

A linked list consists of nodes, as shown below:

![Node](https://i.imgur.com/4MFeYtq.png)

A node contains a Link (the address of the next node) and Data (the stored data). If it's the last node, the next address is NULL. Although we draw it linearly for simplicity, the addresses are actually set randomly. 

Adding a new node involves the following steps. Consider a linked list configured as follows:

![LinkedList](https://i.imgur.com/EUNvMIG.png)

To add a node at the second position:

![LinkedList Add](https://i.imgur.com/3MVrtbF.png)

The deletion process is similar, so it's not shown here. Linked lists avoid the hassle of shifting elements as in arrays.

You can view the C file I wrote for the linked list implementation by clicking the following link. These functions are my creations, though there may be similar code by others. If you use my code, please credit the source.

[LinkedList](https://github.com/justinbrianhwang/A-collection-of-data-structures-and-algorithm-functions/tree/main/linked%20list)

The linked list discussed above is a singly linked list. Let's explore other types of linked lists.

### Types of Linked Lists

- Singly Linked List
- Doubly Linked List
- Circular Linked List

**Doubly Linked List** nodes are structured as follows:

![Doubly](https://i.imgur.com/CEkreJc.png)

Adding or deleting nodes is similar to a singly linked list.

**Circular Linked List** nodes are structured as follows:

![Circle](https://i.imgur.com/x7SDsbz.png)

Adding or deleting nodes is similar to a singly linked list.

You can view the C files I wrote for these linked lists by clicking the following links. These functions are my creations, though there may be similar code by others. If you use my code, please credit the source.

[]()



# Korean

## 리스트

우리가 흔히 사용하는 리스트와 동일한 것이다. 자료를 순서대로 저장하는 자료구조를 의미하며, 일직선으로 연결된 자료이다.

리스트를 구현하기 위해 두 가지 방법이 있다.

- 배열
- 연결리스트

각각의 방법들에 대해 알아보자.

### 배열 리스트

배열의 경우는 메모리에 순차적으로 할당되는 자료구조이므로, 일직선으로 연결됨은 어느 정도 납득이 될 것이다. 그렇다면 순서를 맞추기 위한 알고리즘이 어느 정도 필요할 것이다. 다음과 같이 배열 리스트가 구성이 되어있다고 생각하자.

![array](https://i.imgur.com/fBHK3j8.png)

이렇게 구성된 부분에서 두 번째 위치에 삽입을 한다고 생각하고, 해당 과정을 보도록 하자.

![array move](https://i.imgur.com/Kw4by1r.png)

다음과 같이 배열을 이용한 리스트는 원소를 이동시켜가며 추가해야 한다.

삭제 과정도 보도록 하자.

![array remove](https://i.imgur.com/jNSazoo.png)

다음과 같은 배열 리스트의 두 번째 원소를 삭제하도록 하자.

![array remove2](https://i.imgur.com/WJfzjnO.png)

배열 리스트는 다음 링크를 누르면 내가 짜놓은 C 파일을 볼 수 있을 것이다. 해당 함수들은 내가 만든 것이며, 다른 사람들의 코드를 참고한 적은 없으나, 비슷한 경우가 있을 수는 있다. 내가 짜놓은 코드들을 쓰는 것은 좋으나, 출처를 밝혀주면 좋을 것 같다.

[]()

### 연결 리스트

배열리스트와의 차이점은 제한이 없다는 것이다. 배열의 경우는 크기가 한 번 정해지면 계속해서 변경이 불가능하나, 연결리스트는 이론상으로 무한개를 연결할 수 있다.

**연결리스트의 구조**

‘노드’라는 구조가 있는데, 다음 그림과 같은 자료가 있음을 알고 있으면 된다.

![Node](https://i.imgur.com/4MFeYtq.png)

다음 노드의 주소를 담고 있는 Link와, 자료를 저장하는 Data를 함께 가지고 있는 자료이다. 다음 노드가 없는, 즉 끝 노드라면 다음 주소는 NULL 값을 갖는다. 그림은 일직선으로 그리지만, 사실 다음 노드의 주소는 연속한 형태가 아닌, **랜덤하게 정해지는 것**이다. 하지만 편의를 위해 일직선으로 그릴 것이다.

새로운 노드를 추가하는 경우를 살펴보자.

먼저, 연결리스트의 구성은 다음과 같다고 보자.

![LinkedList](https://i.imgur.com/EUNvMIG.png)

해당 노드 중 두 번째 노드를 추가하는 과정을 작성해보자.

![LinkedList Add](https://i.imgur.com/3MVrtbF.png)

다음과 같은 과정을 통해 추가하는 것이다. 삭제의 과정도 마찬가지이다. 이는 배열과 유사하니, 굳이 남기진 않을 것이다.

배열로 구성한 리스트는 직접 원소를 하나하나 움직인다는 번거로움이 존재하나, 연결리스트는 하나하나 옮기는 과정을 거치지 않아도 된다.

연결 리스트는 다음 링크를 누르면 내가 짜놓은 C 파일을 볼 수 있을 것이다. 해당 함수들은 내가 만든 것이며, 다른 사람들의 코드를 참고한 적은 없으나, 비슷한 경우가 있을 수는 있다. 내가 짜놓은 코드들을 쓰는 것은 좋으나, 출처를 밝혀주면 좋을 것 같다.

[LinkedList](https://github.com/justinbrianhwang/A-collection-of-data-structures-and-algorithm-functions/tree/main/linked%20list)

위에 다룬 연결리스트는 단순 연결리스트였다. 연결리스트의 종류는 여러 가지이다. 이를 살펴보자.

### 연결리스트의 종류

단순 연결리스트

이중 연결리스트

원형 연결리스트

**이중 연결리스트**를 보면 다음과 같은 노드로 구성이 되어있다.

![Doubliy](https://i.imgur.com/CEkreJc.png)

노드의 추가나 삭제의 경우는 단순 리스트와 유사하기에 남기지는 않을 것이다.

**원형 연결리스트**를 보면 다음과 같은 노드로 구성이 되어있다.

![Circle](https://i.imgur.com/x7SDsbz.png)

노드의 추가나 삭제의 경우는 단순 리스트와 유사하기에 남기지는 않을 것이다.

해당 리스트들도 다음 링크를 누르면 내가 짜놓은 C 파일을 볼 수 있을 것이다. 해당 함수들은 내가 만든 것이며, 다른 사람들의 코드를 참고한 적은 없으나, 비슷한 경우가 있을 수는 있다. 내가 짜놓은 코드들을 쓰는 것은 좋으나, 출처를 밝혀주면 좋을 것 같다.

[]()




