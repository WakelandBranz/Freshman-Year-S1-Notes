### 1. Find all integer solutions to each of the following, described in terms of equivalence classes modulo some integer $m \geq 2$. If there are no integer solutions, explain why.

(1) $2x - 4 \equiv 0 \pmod{6}$

$6 \mid (2x-4-0) \to 6 \mid 2(x - 2) \to 2(3) \mid 2(x - 2)$
We can prove that both of these sides have a common factor of 2.
Since $2 \mid 6 = 6/2 = 3$, and 3 is an integer, $2 \mid 6$.
Since $2 \mid 2(x - 2) = \frac{2(x-2)}{2} = x-2,$ $2 \mid 2(x - 2)$.
Both $2 \mid 6$ and $2 \mid 2(x - 2)$ are true, so both sides have a common factor of 2, so we can simplify both sides by dividing 6 by 2 and $2(x - 2)$ by 2.
So, $2(3) \mid 2(x - 2) \to 3 \mid x - 2 \to x - 2 \equiv 0 \pmod 3$
Therefore, $x \equiv 2 \pmod 3$.

(2) $3 + 2x \equiv -2 \pmod{7}$

$7 \mid (3 + 2x + 2) \to 7 \mid (2x + 5) \to 2x + 5 \equiv 0 \pmod{7} \to x \equiv -\frac{1}{2} \pmod 7$



---

### 2. Prove that for all integers $n \geq 0$, $10^n \equiv 1 \pmod{9}$. Then, use that result to show that a positive integer is divisible by 9 if and only if the sum of its digits is divisible by 9.

**-PF-**

WTS that for $n \geq 0$, $10^n \equiv 1 \pmod{9}$ for $n \in \mathbb{Z}$.
So, $10^n \equiv 1 \pmod{9} \iff 10^n \pmod{9} = 1 \pmod{9} = 1$.
From $10^n$ we know $10^n = \underbrace{(10 \times 10 \dots \times 10)}_{\text{n times}}$.
Therefore $10^n \pmod{9} = \underbrace{(10 \times 10 \dots \times 10)}_{\text{n times}} \pmod{9}$
$\implies \underbrace{((10 \pmod{9}) \times (10 \pmod{9}) \dots \times (10 \pmod{9)})}_{\text{n times}} \pmod{9}$
$\implies \underbrace{(1 \times 1 \dots \times 1)}_{\text{ n times}} \pmod{9} = 1$


Now we WTS that for an arbitrary $m$, $m \in \mathbb{Z^+}$, $9 \mid m \iff 9 \mid \text{the sum of m's digits}$.
So, $m \equiv \text{ sum of m's digits} \pmod{9}$.
Let $k =$ the number of $m$'s digits.
We will represent $m$ as its individual digits with $d_{k}$ being the leftmost digit of $m$. 
So, $m = (d_{k} \times 10^k) + (d_{k - 1} \times 10^{k - 1}) \dots + (d_{1} \times 10^1) + (d_{0} \times 10^0).$
If $9 \mid m$, then $m \pmod{9} = [(d_{k} \times 10^k) + (d_{k - 1} \times 10^{k - 1}) \dots (d_{1} \times 10^1), (d_{0} \times 10^0)] \pmod{9} = 0$.
So, $[(d_{k} \times 10^k) \pmod{9} + (d_{k - 1} \times 10^{k - 1}) \pmod{9} \dots + (d_{1} \times 10^1) \pmod{9} + (d_{0} \times 10^0) \pmod{9}] \pmod{9}$
We have proven that any $10^k \pmod{9} = 1$ already, so we can substitute that into our equivalence. 
So $m = [(d_{k} \times 1) + (d_{k - 1} \times 1) \dots (d_{1} \times 1), (d_{0} \times 1)] \equiv 0 \pmod{9}$.
Therefore a positive integer is divisible by 9 if and only if the sum of its digits is divisible by 9.

===FIX THIS ONE===

### Fixed Version

**-PF-**

**Part 1:** We want to show that $10^n \equiv 1 \pmod{9}$ for all $n \geq 0$, where $n \in \mathbb{Z}$.

Note that $10 \equiv 1 \pmod{9}$ since $10 = 9 + 1$.

Now, $10^n = \underbrace{10 \times 10 \times \cdots \times 10}_{n \text{ times}}$.

Therefore, $$10^n \pmod{9} = \underbrace{10 \times 10 \times \cdots \times 10}_{n \text{ times}} \pmod{9}$$

By the multiplicative property of congruences: $$\equiv \underbrace{(10 \pmod{9}) \times (10 \pmod{9}) \times \cdots \times (10 \pmod{9})}_{n \text{ times}} \pmod{9}$$

$$\equiv \underbrace{1 \times 1 \times \cdots \times 1}_{n \text{ times}} \pmod{9} = 1$$

**Part 2:** Now we want to show that for an arbitrary positive integer $m$, we have $9 \mid m \iff 9 \mid \text{(sum of } m\text{'s digits)}$.

Let $k$ be the number of digits in $m$. We represent $m$ using its individual digits, with $d_{k-1}$ being the leftmost digit.

So, $m = (d_{k-1} \times 10^{k-1}) + (d_{k-2} \times 10^{k-2}) + \cdots + (d_1 \times 10^1) + (d_0 \times 10^0)$.

Taking both sides modulo 9: $$m \pmod{9} = [(d_{k-1} \times 10^{k-1}) + (d_{k-2} \times 10^{k-2}) + \cdots + (d_1 \times 10^1) + (d_0 \times 10^0)] \pmod{9}$$

By the additive and multiplicative properties of congruences: $$\equiv [(d_{k-1} \times 10^{k-1}) \pmod{9} + (d_{k-2} \times 10^{k-2}) \pmod{9} + \cdots + (d_1 \times 10^1) \pmod{9} + (d_0 \times 10^0) \pmod{9}] \pmod{9}$$

We have already proven that $10^j \equiv 1 \pmod{9}$ for all $j \geq 0$, so we can substitute: $$m \equiv [(d_{k-1} \times 1) + (d_{k-2} \times 1) + \cdots + (d_1 \times 1) + (d_0 \times 1)] \pmod{9}$$

$$m \equiv d_{k-1} + d_{k-2} + \cdots + d_1 + d_0 \pmod{9}$$

This shows that $m \equiv \text{(sum of digits)} \pmod{9}$.

Therefore, $9 \mid m \iff m \equiv 0 \pmod{9} \iff \text{(sum of digits)} \equiv 0 \pmod{9} \iff 9 \mid \text{(sum of digits)}$.

Thus, a positive integer is divisible by 9 if and only if the sum of its digits is divisible by 9.

---

### 3. Show that if $n$ is any integer, then $n^2$ is congruent modulo 4 to either 0 or 1.

WTS that any integer squared, when$\pmod{4}$ is applied to it, 0 or 1 is always the answer.
Since $n$ is any integer, $\exists k \in \mathbb{Z}$ s.t. $n$ either equals $2k$ or $2k + 1$.
This means that $n^2$ either equals $(2k)^2 = 4k^2$ or $(2k + 1)^2 = 4k^2 + 4k + 1$.
This creates two cases.

Case 1: $n^2 = 4k^2$
Since $n^2 = 4k^2$,  $n^2 \pmod{4} = 4k^2 \pmod{4}$.
Any number multiplied by 4 is divisible by 4, thus  $4k^2 \pmod{4} = 0$ .
So, when $n^2 = 4k^2$, $n^2 \pmod{4} = 0$.

Case 2: $n^2 = 4k^2 + 4k + 1$.
Since $n^2 = 4k^2 + 4k + 1$,  $n^2 \pmod{4} = (4k^2 + 4k + 1) \pmod{4} = [4(k^2 + k) + 1] \pmod{4}$
Any number multiplied by 4 is divisible by 4, thus the modulus of $4(k^2 + k) \pmod{4} = 0$.
But since this number is any arbitrary number multiplied by 4 plus 1, so $[4(k^2 + k) + 1] \pmod{4} = 1$.

Since both cases prove that if $n$ is any integer, then $n^2$ is congruent modulo 4 to either 0 or 1, this holds true.

---

### 4. Use the Euclidean algorithm to find $\gcd(620, 140)$.

Let $a = 620, b = 140$.
$a, b \in \mathbb{Z}$.
Let $q, r \in \mathbb{Z}$ be unique arbitrary numbers s.t. $a = bq + r$.
So, $620 = 140q + r$.
$\to 620 = 140(4) + 60$.
$\to 140 = 60q + r$
$\to 140 = 60(2) + 20$
$\to 60 = 20q + r$
$\to 60 = 20(3) + 0$
Since $r$ is now equal to 0, the algorithm terminates and $gcd(620, 140) = 20$.

---

### 5. Show that an integer $a \in \mathbb{Z}_n$ has a multiplicative inverse, that is, an element $a^{-1} \in \mathbb{Z}_n$ with $a \cdot_n a^{-1} = 1$, if and only if $a$ and $n$ are relatively prime.

---

### 6. The numbers 307 and 220 are relatively prime.

(1) Find integers $x$ and $y$ satisfying $307x + 220y = 1$.

Firstly, use the Euclidian algorithm to prove that these are relatively prime. 
$307 = 220q + r$
$307 = 220(1) + 87$
$220 = 87q + r$
$220 = 87(2) + 46$
$87 = 46q + r$
$87 = 46(1) + 41$
$46 = 41q + r$
$46 = 41(1) + 5$
$41 = 5q + r$
$41 = 5(8) + 1$
$5 = (1)q + r$
$5 = (1)(5) + 0$

Now we will use our Euclidian algorithm in reverse to find integers $x$ and $y$ satisfying $307x + 220y = 1$.
$1 = 41 - 5(8) \rightarrow 1 = 41 - (46 - 41)(8) \to 1 = 9(41) - 8(46)$ $\to 1 = 9(87 - 46) - 8(46) \to 1 = 9(87) - 17(46)$ $\to 1 = 9(87) - 17(220 - 2(87)) \to 1 = 43(87) - 17(220)$ $\to 1 = 43(307 - 220) - 17(220) \to 1 = 43(307) - 60(220) \to 307(43) + 220(-60) = 1$

**Answer: $x = 43, y = -60$**

(2) Use the equation found in (1) to determine the multiplicative inverse of 307 in $\mathbb{Z}_{220}$.

Equation found in 1: $307(43) + 220(-60) = 1$
In $\mathbb{Z_{220}}$, our equation can be represented as $307(43) + 220(-60) \equiv 1 \pmod{220}$.
This can be represented as $307(43) \equiv 1 \pmod{220}$ because $220(-60) \pmod{220} = 0$.
This gives us the multiplicative inverse of $43$ for $307 \in \mathbb{Z_{220}}$.
We can verify this with the following.
$307(43) = 13201$ and $220(-60) = -13200 \to 13201 + (-13200) = 1 \equiv 1 \pmod{220}$.

**Answer:** 43