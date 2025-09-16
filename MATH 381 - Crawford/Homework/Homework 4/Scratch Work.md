### 1. Prove that for integers $a, b,$ and $c$, if $a + b$ and $b + c$ are even, then $a + c$ is even.

**-PF-**
Assume that $a, b, c \in \mathbb{Z}$ and that $a + b$ and $b + c$ are even.
We want to show that $a + c$ is even, meaning $\exists k \in \mathbb{Z}$ such that $a + c = 2k$.
Note $\exists j, l \in \mathbb{Z}$ such that $a + b = 2j$ and $b + c = 2l$.
Therefore $a + b + b + c = 2j + 2l = 2(j + l)$.
Therefore $(a + b) + (b + c) = a + 2b + c \implies a + c = a + 2b + c - 2b = 2(j + l) - 2b = 2(j + l - b)$.
Letting $k = j + l - b$, we see $a + c = 2k$.
So, $k \in \mathbb{Z}$ because $j, l, b \in \mathbb{Z}$.
Thus $a + c$ is even.

---
### 2. Prove that if $x^2 \leq 1$, then $x^2 - 7x > -10$.

**-PF-**
Assume that $x^2 \leq 1$.
Taking the square root of both sides, we get $\sqrt{x^2} \leq \sqrt{1}$ which is equivalent to $|x| \leq 1$.
This means that $-1 \leq x \leq 1$ or $x \in [-1, 1]$.
We want to prove that if $x^2 - 7x > -10$. 
Rearranging the inequality we get $x^2 - 7x + 10 > 0.$
Factoring the left side, we get $(x - 5)(x - 2) > 0$.
In order for this equation to be true, both $(x - 5)$ and $(x - 2)$ must have the same sign since having the same sign would result in a positive number.
Both $(x - 5)$ and $(x - 2)$ have the same sign when $x > 5$ or when $x < 2$.
Since we have $-1 \leq x \leq 1$, we know that both $(x - 5) < 0$ and $(x - 2) < 0$.
Thus $(x - 5)(x - 2) > 0$.
Therefore $x^2 - 7x > -10$.

---
### 3. Prove that if $a^2 + b^2 = c^2$, then $abc$ is even, where $a,b,c$ are any integers.

===Ask Matt about the proof to this problem. I looked it up and it makes some sense, but I want to know more about pattern recognition on when to use modulus for proofs because it seems like a very valuable tool which I know how to use but I don't know when to use it.===

**-PF-**
Assume that $a^2 + b^2 = c^2$ and $a, b , c \in \mathbb{Z}$. 
We want to show that $abc$ is even, meaning that $\exists k \in \mathbb{Z}$ such that $abc = 2k$.
No idea where to go with this. Try contradiction.

**-PF-**
Assume that $a^2 + b^2 = c^2$ and $a, b , c \in \mathbb{Z}$. 
By contradiction, we want to show that $abc$ is odd.
This means that a, b, and c are all odd, since if any a, b, or c was even then the product of $abc$ would be even.
If $a$ is odd, then $\exists k \in \mathbb{Z}$ such that $a = 2k + 1$.
Therefore, $a^2 = (2k + 1)(2k + 1) = 4k^2 + 4k + 1$. 
Using this, we can deduce $4k^2 + 4k + 1 \equiv 1 \pmod{4}$.
By the same logic and continuing the same assumption that a, b, and c are all odd, we can similarly deduce that $b^2 \equiv 1 \pmod4$ and $c^2 \equiv 1 \pmod4$ 

---
### 4. Suppose that $x$ and $y$ are real numbers. Prove that if $x + y$ is irrational then $x$ is irrational or $y$ is irrational.

**-PF-**
Assume that $x, y \in \mathbb{R}$.
We want to show that $x + y$ is irrational  

---
### 5. Prove that there are no positive integer solutions to $x^2 + x + 1 = y^2$

**-PF-**

---
### 6. Prove that $\sqrt[3]2$ is irrational.

Notes: 
$gcd(a, b) =$ a & b are coprime $= a \perp b$

**-PF-**
Assume for contradiction that $\sqrt[3]{2}$ is rational.
Then $\exists a, b \in \mathbb{Z}$ and $b \neq 0$ where a and b are coprime such that $\sqrt[3]{2} = \frac{a}{b}$.
Cubing both sides we get $2 = (\frac{a}{b})^3 = \frac{a^3}{b^3}$.
Therefore $2b^3 = a^3$.
This means that $a^3$ is even which implies that $a$ is also even.
Assume $\exists k \in \mathbb{Z}$ such that $a = 2k$.
Therefore $a^3 = (2k)^3 = 8k^3$.
Therefore $4k^3 = b^3 = 2(2k^3)$.
This means that $b^3$ is even which implies that $b$ is also even.
Since both $a$ and  are even, then the prior assumption that a and b are coprime is contradicted because they also share a common factor of 2.
Therefore $\sqrt[3]{2}$ is irrational.

---
### 7. Show that the following statement about the real numbers $a$ and $b$ are equivalent:

#### (a) $a < b$

**-PF-**

---
#### (b) $(a + b)/2 > a$

**-PF-**

---
#### (c) $(a + b)/2 < b$

**-PF-**

---
### 8. Prove that either $2 * 10^500 + 15$ or $2 * 10^500 + 16$ is not a perfect square.

**-PF-**

---
### 9. Prove or disprove: If $x$ and $y$ are rational numbers, then $x^y$ must be rational.

**-PF-**