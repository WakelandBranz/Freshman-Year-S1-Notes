### 1. Find all integer solutions to each of the following, described in terms of equivalence classes modulo some integer $m \geq 2$. If there are no integer solutions, explain why.

(1) $2x - 4 \equiv 0 \pmod{6}$

(2) $3 + 2x \equiv -2 \pmod{7}$

---

### 2. Prove that for all integers $n \geq 0$, $10^n \equiv 1 \pmod{9}$. Then, use that result to show that a positive integer is divisible by 9 if and only if the sum of its digits is divisible by 9.

---

### 3. Show that if $n$ is any integer, then $n^2$ is congruent modulo 4 to either 0 or 1.

WTS that any integer squared, when$\pmod{4}$ is applied to it, 0 or 1 is always the answer.
Since $n$ is any integer, $\exists k \in \mathbb{Z}$ s.t. $n$ either equals $2k$ or $2k + 1$.
This means that $n^2$ either equals $(2k)^2 = 4k^2$ or $(2k + 1)^2 = 4k^2 + 4k + 1$.
This creates two cases.
Case 1: $n^2 = 4k^2$
Since $n^2 = 4k^2$,  $n^2 \pmod{4} = 4k^2 \pmod{4}$.
Any number multiplied by 4 is divisible by 4, thus the modulus of said number is equal to 0.
So, when $n^2 = 4k^2$, $n^2 \pmod{4} = 0$.
Case 2: $n^2 = 4k^2 + 4k + 1$.
Since $n^2 = 4k^2 + 4k + 1$,  $n^2 \pmod{4} = (4k^2 + 4k + 1) \pmod{4}$
Any number multiplied by 4 is divisible by 4, thus the modulus of said number is equal to 0.

---

### 4. Use the Euclidean algorithm to find $\gcd(620, 140)$.

---

### 5. Show that an integer $a \in \mathbb{Z}_n$ has a multiplicative inverse, that is, an element $a^{-1} \in \mathbb{Z}_n$ with $a \cdot_n a^{-1} = 1$, if and only if $a$ and $n$ are relatively prime.

---

### 6. The numbers 307 and 220 are relatively prime.

(1) Find integers $x$ and $y$ satisfying $307x + 220y = 1$.

(2) Use the equation found in (1) to determine the multiplicative inverse of 307 in $\mathbb{Z}_{220}$.