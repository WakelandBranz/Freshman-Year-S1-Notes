### 1.

Prove the inequality $n < 2^n$ for all positive integers $n$.

**-PF-**

WTS $n < 2^n$ for all positive integers $n$.
Base case: When $n = 1$, $n < 2^n \to 1 < 2^1 \to 1 < 2$ which is true.
Inductive step: Assume $k < 2^k$ for $k \in \mathbb{Z^+}, k \geq 1$.
WTS $k + 1 < 2^{k + 1}$.
Note: $k \geq 1$
$$k + 1 < 2^k + 1 < 2^k + 2^k$$
$$\to k + 1 < 2^k + 1 < 2(2^k)$$
$$\to k + 1 < 2^k + 1 < 2^{k + 1}$$
$$\to k + 1 < 2^{k + 1}$$
By mathematical induction, $n < 2^n$ for all positive integers $n$.

---

### 2.

rove that $7^{n+2} + 8^{2n+1}$ is divisible by 57 for every nonnegative integer $n$.

**-PF-**

WTS $57 \mid 7^{n + 2} + 8^{2n + 1}$ for all $n \in \mathbb{Z}, n \geq 0$.
**Base cases:** 
For $n = 0, 7^{n + 2} + 8^{2n + 1} \to 7^2 + 8^1 = 57$
$57 \pmod{57} = 0$ thus $57 \mid 57$ so this case is valid.
**Inductive step:** Assume that $57 \mid 7^{k + 2} + 8^{2k + 1}$ for $k \in \mathbb{Z}, k \geq 0$.
WTS that $57 \mid 7^{k + 1 + 2} + 8^{2(k + 1) + 1} \to 57 \mid 7^{k + 3} + 8^{2k + 3}$.
From the inductive hypothesis we can deduce $7^{k + 2} + 8^{2k + 1} \equiv 0 \pmod{57}$.
So, $7^{k + 2} \equiv -8^{2k + 1} \pmod{57}$.
Furthermore, we can deduce that $7^{k + 3} + 8^{2k + 3} = 7(7^{k + 2}) + 64(8^{2k + 1})$.
So, substituting $-8^{2k + 1} \pmod{57}$ for $7^{k + 2} \pmod{57}$ we can find the following: $$7(7^{k + 2}) + 64(8^{2k + 1}) \equiv 7(-8^{2k + 1}) + 64(8^{2k + 1}) \pmod{57}$$
Simplifying, we find the following:
$$\equiv 57(8^{2k + 1}) \pmod{57}$$
Any arbitrary number multiplied by $57 \pmod{57}$ is equivalent to 0.
This means that $57 \mid 7^{k + 3} + 8^{2k + 3}$.
By mathematical induction, $57 \mid 7^{n + 2} + 8^{2n + 1}$ for all $n \in \mathbb{Z}, n \geq 0$.

---

### 3.

Prove the early proposition that $|P(S)| = 2^n$ where $|S| = n$.

---

### 4.

Prove that $n! < n^n$ for all integers $n > 1$.

(The notation $n!$ is the product of all positive integers less than or equal to $n$. Ex: $5! = 5 \cdot 4 \cdot 3 \cdot 2 \cdot 1 = 120$)

**-PF-**

WTS $n! < n^n$ for all integers $n > 1$.
Base case: 
$n = 2, 2! < 2^2 \to 2 < 4$, this is valid.
Assume that for some arbitrary integer $k > 1$, $k! < k^k$.
WTS $(k + 1)! < (k + 1)^{k + 1}$.
Since $k < k + 1$ and $k > 1$, we have $k^k < (k + 1)^k$.
From this we can deduce that $k! < k^k < (k + 1)^k$ so $k! < (k + 1)^k$.
$(k + 1)!$ can be represented as $(k + 1) \cdot (k!)$.
$(k + 1)^{k + 1}$ can be represented as $(k + 1)\cdot (k + 1)^k$.
Since both expressions differ only by a positive factor of $(k + 1)$, and we know $k! < (k + 1)^k$, it follows that $(k + 1)! < (k + 1)^{k + 1}$.
Therefore, by mathematical induction, $n! < n^n$ for all integers $n > 1$.

---

### 5.

Prove that any amount of postage $n \geq 18$ can be formed using only 4-cent 
and 7-cent stamps.

**-PF-**

WTS that any amount of postage $n \geq 18$ can be formed using only 4-cent and 7-cent stamps.
Base cases:
$n = 18, 18 = 7(2) + 4(1)$, this is valid.
$n = 19, 19 = 7(1) + 4(3)$, this is valid.
$n = 20, 20 = 7(0) + 4(5)$, this is valid.
$n = 21, 21 = 7(3) + 4(0)$, this is valid.
Assume for all $j, k \in \mathbb{Z}^+, j, k \geq 18$, $18 \leq j \leq k$ can be formed using only 4-cent and 7-cent stamps.
WTS that $k + 1$ can be formed using only 4-cent and 7-cent stamps.
For $k \geq 21$, we know that $k - 3$ can be formed using only 4-cent and 7-cent stamps because it falls within $j$.
So, $k + 1 = (k - 3) + 4$ can be formed by taking the stamp combination for $k - 3$ (which falls within our inductive hypothesis' range) plus a 4-cent stamp, meaning that $k + 1$ can be formed using only 4-cent and 7-cent stamps.
Therefore, by mathematical induction, any amount of postage $n \geq 18$ can be formed using only 4-cent and 7-cent stamps.

---

### 6.

Prove that every positive integer can be written as a sum of distinct powers of 2.

(This is why binary code works. Ex: $3 = 2^1 + 2^0$, $11 = 2^3 + 2^1 + 2^0$, $30 = 2^4 + 2^3 + 2^2 + 2^1$)

**-PF-**

WTS that every positive integer can be written as a sum of distinct powers of 2.
***Base cases:***
$n = 1, 2^0 = 1$, this is valid.
Assume $j \in \mathbb{Z}^+$ with $1 \leq j \leq k$ and that our proposition holds for $j$.
WTS, for $k \in \mathbb{Z}^+$, that $k + 1$ can be written as a sum of distinct powers of 2.
This creates two cases.
Case 1: $k + 1$ is even.
Since $k + 1$ is even, we know that $\frac{k + 1}{2} \in \mathbb{Z}^+$.
From our inductive hypothesis, we know that $1 \leq \frac{k + 1}{2} \leq k + 1$ meaning that $\frac{k + 1}{2}$ can be represented as a sum of distinct powers of 2.
Multiplying $\frac{k+ 1}{2}$ by 2 results in $k + 1$, but this simply results in each distinct power of 2 which sums to equal $k + 1$ having its exponent increased by 1, thus allowing it to remain distinct.
Case 2: $k + 1$ is odd.
We know that $k + 1$ is odd, so $k$ must be even.
Using our inductive hypothesis, we know that $k$ can be represented as the sum of distinct powers of 2 since $j \leq k$.
Since $k$ is even, its sum of distinct powers of 2 does not include $2^0$, thus $k + 1$ can be represented as $k + 2^0$ and it remains a sum of distinct powers of 2.
Thus, by mathematical induction, every positive integer can be written as a sum of distinct powers of 2.

---

### 7.

Define a sequence of numbers as follows: Let $a_0 = 3$ and $a_1 = 7$ and for $n \geq 2$, let $a_n = 6a_{n-1} - 5a_{n-2}$.

#### (a)

Determine $a_2$, $a_3$ and $a_4$.

$a_n = 6a_{n - 1} - 5a_{n - 2}$
$a_2 = 6a_{1} - 5a_{0} = 6(7) - 5(3) = 27$
$a_3 = 6a_{2} - 5a_{1} = 6(27) - 5(7) = 127$
$a_4 = 6a_{3} - 5a_{2} = 6(127) - 5(27) = 627$

$a_5 = 6a_4 - 5a_3 = 6(627) - 5(127) = 3127$
$a_6 = 6a_5 - 5a_4 = 6(3127) - 5(627) = 15627$
$a_7 = 6a_6 - 5a_5 = 6(15627) - 5(3127) = 78127$
#### (b)

Conjecture a formula for $a_n$ which is not defined recursively. (Such as $a_n = n^2 + 1$.)

$a_{n} = 5^n + 2$

Saw a pattern in the equations that $5^n = a_n - 2$ so I discovered algebraically that $a_n = 5^n + 2$.
#### (c)

Prove your formula using strong induction.

**-PF-**

WTS that $a_n = 5^n + 2$ is equivalent to the recursive formula $a_n = 6a_{n - 1} - 5a_{n - 2}$ for all $n \in \mathbb{Z}, n \geq 0$.
***Base cases:***
$n = 0, a_0 = 5^0 + 2 = 3$, this is true.
$n = 1, a_1 = 5^1 + 2 = 7$, this is true.
Assume that for all integers $j$ with $0 \leq j \leq k$ (where $k \geq 1$), we have $a_j = 5^j + 2$.
WTS $a_{k + 1} = 5^{k + 1} + 2$ is equivalent to the recursive formula $a_{k + 1} = 6a_k - 5a_{k - 1}$.
Note, $5^{k + 1} + 2 = 5(5^k) + 2$.
From the inductive hypothesis we know that $a_k = 5^k + 2$ and $a_{k - 1} = 5^{k - 1} + 2$.
So, substituting these into our recursive formula we get $$a_{k + 1} = 6(5^k + 2) - 5(5^{k - 1} + 2) = 6 \cdot 5^k + 12 - 5^k - 10 = 5 \cdot 5^k + 2 = 5^{k + 1} + 2$$
From this substitution we know that $5^{k + 1} + 2 = a_{k + 1}$ so this proves our inductive hypothesis.
Thus, via strong induction, $a_n = 5^n + 2$ is equivalent to the recursive formula $a_n = 6a_{n - 1} - 5a_{n - 2}$.