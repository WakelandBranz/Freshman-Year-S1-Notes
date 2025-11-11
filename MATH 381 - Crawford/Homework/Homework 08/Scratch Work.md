### 1.

Prove the inequality $n < 2^n$ for all positive integers $n$.

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

Prove that $7^{n+2} + 8^{2n+1}$ is divisible by 57 for every nonnegative integer $n$.

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


# wrong
$7^{k + 3}$ can be represented as $7(7^k \cdot 49) \to 343(7^k).$
$8^{2k + 3}$ can be represented as $8(8^{2k} \cdot 64) \to 512(8^{2k})$.
$343 \equiv 1 \pmod{57}$.
Since $343(7^k)$ is a multiple of $343$, $343(7^k) \equiv 1 \pmod{57} = 343 \equiv 1 \pmod{57}$.
$512 \equiv 56 \pmod{57}$.
Since $512(8^{2k})$ is a multiple of 512, $512(8^{2k}) \equiv 56 \pmod{57} = 512 \equiv 56 \pmod{57}$.
From this, we can deduce that $[343(7^k) + 512(8^{2k})] \pmod{57} = (343 + 512) \pmod{57}$.
$343 + 512 \equiv 0 \pmod{57}$.
Therefore, for all $k \in \mathbb{Z}, k \geq 0$, $57 \mid 7^{k + 3} + 8^{2k + 3}$.

---

### 3.

Prove the early proposition that $|P(S)| = 2^n$ where $|S| = n$.

WTS that $|P(S)| = 2^n$ where $|S| = n$.
*Base case:* $n = 0$
When $n = 0$, then $|S| = 0$ thus $S = \emptyset$.
So, $P(\emptyset) = \set{\emptyset}$.
So $|P(\emptyset)| = 1 = 2^0.$
*Inductive step:* Let $n \geq 0$ and assume that for any set $S$ with $|S| = n$, we have $|P(S)| = 2^n$.
Now consider a set $K$ with $|K| = n + 1$.
Since $K$ is nonempty, we can find an element $x  \in K$.


---

### 4.

Prove that $n! < n^n$ for all integers $n > 1$.

(The notation $n!$ is the product of all positive integers less than or equal to $n$. Ex: $5! = 5 \cdot 4 \cdot 3 \cdot 2 \cdot 1 = 120$)

WTS $n! < n^n$ for all integers $n > 1$.
Base case: $n = 2 \to 2! < 2^2 \to 2 < 4$ which is true.
Inductive hypothesis: Assume that for some arbitrary integer $k > 1$, $k! < k^k$.
WTS $(k + 1)! < (k + 1)^{k + 1}$.
For all $k$, $(k + 1)!$ can be represented as the following:
$$\underbrace{(k  + 1) \cdot (k) \cdot k - 1 \dots 2 \cdot 1}_{\text{k + 1 times}}$$
For all $k$, $(k + 1)^{k + 1}$ can be represented as the following:
$$\underbrace{(k + 1) \cdot (k + 1) \cdot (k + 1) \dots (k + 1)}_{\text{k + 1 times}}$$
===FIX THIS SENTENCE!!!!=== Since $k > 1$, $(k + 1)^{k + 1} > (k + 1)!$ because both sides of the inequality are multiplied $k + 1$ times but $(k + 1)^{k + 1}$ is always multiplied by larger numbers than $(k + 1)!$.
Therefore, by induction, $n! < n^n$ for all integers $n > 1$. 

---

### 5.

Prove that any amount of postage $n \geq 18$ can be formed using only 4-cent and 7-cent stamps.

===FIX UP THIS LOGIC===

WTS $n \geq 18$ can be formed using only 4-cent and 7-cent stamps.
Base cases: 
$n = 18$ can be formed with 2 7-cent stamps and 1 4-cent stamp $\to 18 = 7(2) + 4(1)$.
$n = 19$ can be formed with 1 7-cent stamp and 3 4-cent stamps $\to 19 = 7(1) + 4(3)$.
$n = 20$ can be formed with 5 4-cent stamps $\to 20 = 7(0) + 4(5)$.
$n = 21$ can be formed with 3 7-cent stamps $\to 21 = 3(7) + 4(0)$.
Let there be arbitrary integers $k, j$ s.t. $k \geq 21$ and $18 \leq j \leq k + 1$.
Assume that for all $j$ where $18 \leq j \leq k$, we can form $j$ using 4-cent and 7-cent stamps.
WTS $18 \leq j \leq k + 1$ allows $j$ to be formed using 4-cent and 7-cent stamps.
So, $18 \leq (k + 1) - 4 \to 18 \leq k - 3$ which tells us that by adding 1 4-cent stamp we can represent $k + 1$.
By induction, $n \geq$ can be formed using only 4-cent and 7-cent stamps.

---

### 6.

Prove that every positive integer can be written as a sum of distinct powers of 2.

(This is why binary code works. Ex: $3 = 2^1 + 2^0$, $11 = 2^3 + 2^1 + 2^0$, $30 = 2^4 + 2^3 + 2^2 + 2^1$)

**-PF-**
WTS that every positive integer can be written as a sum of distinct powers of 2.
***Base cases:***
$n = 1, 1 = 2^0$ thus for $n = 1$ this is true.
Assume that for all positive integers $k$ (where $k \geq 1$), $k$ can be written as a sum of distinct powers of 2.
WTS $k + 1$ can be written as a sum of distinct powers of 2.
Note, $1 = 2^0$.
This creates two cases.
Since we want to prove $k + 1$ can be written as a sum of distinct powers of 2, we can substitute $2^0$ for 1 which results in $k + 2^0$.
This creates two cases.
Case 1: $k$ is not written with $2^0$ as a sum of its distinct powers of 2.
In this case, $k + 1$ can be represented as $k + 2^0$ and since we know that $k$ can already be written as a sum of distinct integers, $k + 1$ can also be written as a sum of distinct powers of 2.
Case 2: $k$ is written with $2^0$ as a sum of its distinct powers of 2.
In this case, writing $k + 1$ as $k + 2^0$ would result in $k + 1$ not being represented by a sum **distinct** powers of 2.
Despite this, 


Therefore, by mathematical induction, every positive integer can be written as a sum of distinct powers of 2.


$n = 2, 2 = 2^1$ thus for $n = 2$ this is true.
$n = 3, 3 = 2^1 + 2^0$ thus for $n = 3$ this is true.
$n = 4, 4 = 2^2$ thus for $n = 4$ this is true.
*Inductive Hypothesis:* Let there exist an arbitrary $k, j \in \mathbb{Z}^+$ s.t. $1 \leq j \leq k$ 

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
Thus, via strong induction $a_n = 5^n + 2$ is equivalent to the recursive formula $a_n = 6a_{n - 1} - 5a_{n - 2}$.

---

### 8. Optional

The Fibonacci sequence is defined recursively as: $$F_1 = 1, F_2 = 1; \quad F_n = F_{n-1} + F_{n-2} \text{ for } n \geq 2$$

#### (a)

Write down the first several terms in the Fibonacci sequence.

0, 1, 2, 3, 5, 8, 13, 21

#### (b)

Prove that for $n \geq 3$, $F_n \geq \alpha^{n-2}$ where $\alpha = \frac{1+\sqrt{5}}{2}$.