### 1.

Prove the inequality $n < 2^n$ for all positive integers $n$.

1. WTS $n < 2^n$, $\forall n \in \mathbb{Z^+}$.
2. Base case: When $n = 1$, $n < 2^n \to 1 < 2^1 \to 1 < 2$ which is true.
3. Inductive step: Assume $k < 2^k$ for $k \in \mathbb{Z^+}, k \geq 1$.
4. WTS $k + 1 < 2^{k + 1}$.
5. By the inductive hypothesis:
Note: $k \geq 1$
$$k + 1 < 2^k + 1 < 2^k + 2^k$$
$$\to k + 1 < 2^k + 1 < 2(2^k)$$
$$\to k + 1 < 2^k + 1 < 2^{k + 1}$$
From this, we can deduce the following: 
$$\to k + 1 < 2^{k + 1}$$

---

### 2.

Prove that $7^{n+2} + 8^{2n+1}$ is divisible by 57 for every nonnegative integer $n$.

---

### 3.

Prove the early proposition that $|P(S)| = 2^n$ where $|S| = n$.

---

### 4.

Prove that $n! < n^n$ for all integers $n > 1$.

(The notation $n!$ is the product of all positive integers less than or equal to $n$. Ex: $5! = 5 \cdot 4 \cdot 3 \cdot 2 \cdot 1 = 120$)

---

### 5.

Prove that any amount of postage $n \geq 18$ can be formed using only 4-cent and 7-cent stamps.

---

### 6.

Prove that every positive integer can be written as a sum of distinct powers of 2.

(This is why binary code works. Ex: $3 = 2^1 + 2^0$, $11 = 2^3 + 2^1 + 2^0$, $30 = 2^4 + 2^3 + 2^2 + 2^1$)

---

### 7.

Define a sequence of numbers as follows: Let $a_0 = 3$ and $a_1 = 7$ and for $n \geq 2$, let $a_n = 6a_{n-1} - 5a_{n-2}$.

#### (a)

Determine $a_2$, $a_3$ and $a_4$.

#### (b)

Conjecture a formula for $a_n$ which is not defined recursively. (Such as $a_n = n^2 + 1$.)

#### (c)

Prove your formula using strong induction.

---

### 8. Optional

The Fibonacci sequence is defined recursively as: $$F_1 = 1, F_2 = 1; \quad F_n = F_{n-1} + F_{n-2} \text{ for } n \geq 2$$

#### (a)

Write down the first several terms in the Fibonacci sequence.

#### (b)

Prove that for $n \geq 3$, $F_n \geq \alpha^{n-2}$ where $\alpha = \frac{1+\sqrt{5}}{2}$.