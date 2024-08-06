# English

### Definition of Structures

A data type that groups together different data types into a single unit.

![struct](https://i.imgur.com/Wa4H1Fr.png)

### Dynamic Memory Allocation using Pointers

- Allocating memory dynamically during program execution.
- Dynamic: The size of the memory to be allocated is not predetermined at compile time.

**Disadvantages**

- More difficult to use compared to static memory allocation.
- Memory must be explicitly freed after use.
- Potential for memory leaks.

### Static Memory Allocation

- Memory size to be allocated is predetermined before the program runs.

### Dynamic Memory Allocation Functions

- `malloc()`: Allocates memory.
- `free()`: Frees allocated memory.
- `memset()`: Initializes memory.

### Declaration and Definition of Arrays

Declaration

- Indicates the name without assigning a memory address.
- Example: `int a, int x();`

Definition

- Assigns a memory address to the declared name.

Array Declaration

- `a[n]`
- `a`: Name of the array
- `n`: Maximum number of elements

### 1D Representation

**Memory Representation**

- Consecutive memory addresses are allocated to the array.
- Elements are stored sequentially within the allocated memory.
- Sequential mapping: Logical order of the array matches the physical order in memory.
- Sequential representation: Using sequential mapping to represent data.

**Array Definition**

- A data type that stores elements of the same type sequentially in memory.

![arr1](https://i.imgur.com/0Tv0juC.png)

### 2D Representation

Array Declaration

- `a[n1][n2]`
- `n1`: Number of rows
- `n2`: Number of columns
- Number of elements: `n1` ⨉ `n2`

Memory Representation

- Row-major order: The general method
- Column-major order

![arr2](https://i.imgur.com/cTvZl4o.png)

### 3D Representation

Array Declaration

- `a[n1][n2][n3]`
- `n1`: Number of planes
- `n2`: Number of rows
- `n3`: Number of columns
- Number of elements: `n1` ⨉ `n2` ⨉ `n3`

Memory Representation

- Sequentially mapping `n1` 2D arrays into 1D memory.

![arr3](https://i.imgur.com/0FFjzFS.png)


# Korean

### 구조체의 정의

서로 다른 자료형의 데이터를 하나의 그룹으로 묶은 자료형 

![struct](https://i.imgur.com/Wa4H1Fr.png)

### 포인터를 이용한 동적 메모리 할당

- 프로그램 실행 도중 동적으로 메모리를 할당하는 것
- 동적: 할당될 메모리의 크기가 컴파일할 때 미리 정해져 있지 않았다는 의미

**단점**

- 사용 방법이 정적 메모리 할당에 비해 다소 어려움
- 메모리를 다 사용한 다음 반드시 메모리를 해제시켜 주어야 함
- 메모리 누수

### 정적 메모리 할당

- 프로그램이 실행되기 전에 할당해야 할 메모리 크기가 미리 정해진 경우

### 동적 메모리 할당 함수

- `malloc()`: 메모리 할당
- `free()`: 메모리 해제
- `memset()`: 메모리 초기화

### 배열의 선언 및 정의

선언

- 메모리 상의 주소가 정해지지 않고 이름만 알려줌
- `int a, int x();` 등등

정의

- 대상의 이름에 대해 대응하는 메모리 상의 주소가 정해지는 것

배열의 선언

- `a[n]`
- `a`: 배열의 이름
- `n`: 원소 최대 수

### 1차원 표현

**메모리 표현**

- 연속적인 메모리 주소를 배열에 할당
- 원소는 할당된 메모리 내에서 인덱스 순서에 따라 저장
- 순차사상: 배열의 논리적 순서와 메모리의 물리적 순서가 같도록 표현
- 순차표현: 순차 사상을 이용하여 데이터를 표현

**배열의 정의**

- 같은 자료형의 데이터를 메모리 상에 연속적으로 저장하는 자료형 

![arr1](https://i.imgur.com/0Tv0juC.png)

### 2차원 표현

배열의 선언

- `a[n1][n2]`:
- `n1`: 행의 수
- `n2`: 열의 수
- 원소 수: `n1` ⨉ `n2`

메모리 표현

- 행 우선 순서: 일반적인 방법
- 열 우선 순서

![arr2](https://i.imgur.com/cTvZl4o.png)

### 3차원 표현

배열의 선언

- `a[n1][n2][n3]`
- `n1`: 면의 수
- `n2`: 행의 수
- `n3`: 열의 수
- 원소 수:  `n1` ⨉ `n2` ⨉ `n3`

메모리 표현

- `n1`개의 2차원 배열을 차례로 1차원 메모리에 순차 사상하는 방법

![arr3](https://i.imgur.com/0FFjzFS.png)
