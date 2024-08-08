# Korean

## Basic Probability Theory

### Probability

The degree to which an event is likely to happen

![dice coin](https://i.imgur.com/G7e9wq3.png)

The probability that a die is an even number, or that two coins come up heads at least once when flipped.

## Glossary of terms

### Probability Experiments

- You don't know the outcome of your experiment in advance.
- All possible outcomes of an experiment are known in advance.
- In theory, you can repeat the experiment.

### Sample Space

- A meeting of all results

### Source event

- Elements in Sample Space

### Events

- Sample space is a subset, a set of underlying events
### Treachery Incidents

- Events whose intersection is a union


## Representing probability symbols

- The degree to which an event is likely to happen
- $P(x)$
- Source event: $A$, sample space: $S$

$0 \leq P(A) \leq 1$

$P(S) = 1$

$P(A) = {n(A)\over n(S)}$

![pro](https://imgur.com/12ac56b4-b2f6-43a3-8fec-9f9f879011a8)

### Conditional probability

Given event $A$, the probability that event $B$ is corrected

↔ Given $A$, the probability of $B$ happening

$$
P(B|A) = {P(A \cap B)\over P(A)}
$$

### Independent

Events $A$ and $B$ are independent events if they have no effect on each other. 

⇒ In fact, conditional probability and its use in Bayes' theorem are some of the most important concepts in AI. We'll cover Bayes' theorem in more detail in the next chapter.




---

# Korean

## 확률 기본 이론

### 확률

어떤 사건이 일어날 가능성의 정도

![dice coin](https://i.imgur.com/G7e9wq3.png)

주사위가 짝수일 확률 or 두 개의 동전을 던질 때 앞면이 한번이라도 나올 경우

## 용어 정리

### 확률 실험

- 실험 결과를 미리 알 수 없다.
- 실험에서 일어날 수 있는 모든 결과는 사전에 알려져 있다.
- 이론적으로는 실험을 반복할 수 있다.

### 표본 공간

- 모든 결과들의 모임

### 근원 사건

- 표본 공간의 원소

### 사건

- 표본 공간이 부분 집합, 근원 사건의 집합

### 배반 사건

- 서로 교집합이 공집합인 사건

## 확률 기호 표기

- 어떠한 사건이 일어날 가능성의 정도
- $P(x)$
- 근원 사건: $A$, 표본 공간: $S$

$0 \leq P(A) \leq 1$

$P(S) = 1$

$P(A) = {n(A)\over n(S)}$

![pro](https://imgur.com/12ac56b4-b2f6-43a3-8fec-9f9f879011a8)

### 조건부 확률

사건 $A$가 주어질 때, 사건 $B$가 교정이 된 확률

↔ $A$가 주어졌을 때, $B$가 일어날 확률

$$
P(B|A) = {P(A \cap B)\over P(A)}
$$

### 독립

사건 $A$와 사건 $B$가 서로에게 아무런 영향을 미치지 않을 때, 사건 $A$와 $B$는 독립사건이다. 

⇒ 사실 인공지능에서 조건부확률과, 이를 이용한 베이즈 정리가 제일 중요한 개념들이다. 다음 챕터에서 베이즈 정리에 대해 자세히 다뤄보자.
