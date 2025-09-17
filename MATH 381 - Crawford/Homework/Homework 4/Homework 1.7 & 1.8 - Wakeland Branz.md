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
<div style="page-break-after: always;"></div>
page break above me

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
### 3. COMPLETE THIS RETARD


---
### 4. Suppose that $x$ and $y$ are real numbers. Prove that if $x + y$ is irrational then $x$ is irrational or $y$ is irrational.

**-PF-**
Assume that $x, y \in \mathbb{Q}$. 
We want to find, by contraposition, that if $x$ and $y$ are rational then $x + y$ is also rational.
Then, $\exists a, b, c, d \in \mathbb{Z}$ with $b, d \neq 0$ such that $x = \frac{a}{b}$ and $y = \frac{c}{d}$ with all common factors of $\frac{a}{b}$ and $\frac{c}{d}$ cancelled.
Note, $x + y = \frac{a}{b} + \frac{c}{d} = \frac{ad + bc}{bd}$ and $ad + bc$ and $bd$ are integers and $bd \neq 0$ because neither $b$ nor $d$ were 0.
Thus, by contraposition, if $x + y$ is irrational, then $x$ is irrational or $y$ is irrational.

---
### 5. Prove that there are no positive integer solutions to $x^2 + x + 1 = y^2$

**-PF-**
Assume, for contradiction, $\exists x,y \in \mathbb{Z}^+$ such that $x^2 + x + 1 = y^2$.
Subtracting 1 from both sides we get $x^2 + x = y^2 - 1$.
Simplifying this we get $x^2 + x = (y + 1)(y - 1) = x(x + 1)$.
So, $x(x + 1) = (y + 1)(y - 1)$.
So, given $x \in \mathbb{Z}^+$, $x^2 < x^2 + x + 1 = y^2$ which implies $x^2 < y^2$ which implies $x < y$. 
Comparing $x^2 + x + 1$ to the next perfect square yields $x^2 + x + 1 < x^2 + 2x + 1$ which is true given that $x \in \mathbb{Z}^+$. 
Simplifying we get $x + 1 < 2x + 1 \equiv 0 < x$ which is true given that $x \in \mathbb{Z}^+$.
Therefore $y^2 = x^2 + x + 1 < (x + 1)^2$ which implies $y < x + 1$.
Using this we discover $x < y < x + 1$.
This is a contradiction because $x, y \in \mathbb{Z}^+$ but $y$ cannot be an integer in order for $x < y < x + 1$ to hold true.
Thus there are no positive integer solutions to $x^2 + x + 1 = y^2$.

---
### 6. Prove that $\sqrt[3]2$ is irrational.

Notes: 
$gcd(a, b) || gcf(a,b) =$ a & b are coprime $= a \perp b$

**-PF-**
Assume for contradiction that $\sqrt[3]{2}$ is rational.
Then $\exists a, b \in \mathbb{Z}$ and $b \neq 0$ such that $\sqrt[3]{2} = \frac{a}{b}$ with all common factors of $a$ and $b$ cancelled.
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
#### (b) $(a + b)/2 > a$
#### (c) $(a + b)/2 < b$

**-PF-**
We want to show that $a \implies b \implies c \implies a$.
$(a \implies b)$: $a < b \equiv 2a < a + b \equiv a < \frac{a + b}{2} \equiv \frac{a + b}{2} > a$
$(b \implies c)$: $\frac{a + b}{2} > a \equiv a + b > 2a \equiv b > a \equiv 2b > a + b \equiv b > \frac{a + b}{2} \equiv \frac{a + b}{2} < b$
$(c \implies a)$: $\frac{a + b}{2} < b \equiv a + b < 2b \equiv a < b$
This shows that (a), (b), (c) are all equivalent inequalities.

---
### 8. COMPLETE THIS RETARD!

---
### 9. Prove or disprove: If $x$ and $y$ are rational numbers, then $x^y$ must be rational.

**-PF-**
This statement is false.
This can be proven by a counterexample where $x = 2$ and $y = 1/2$.
When $x = 2$ and $y = 1/2$, $x, y \in \mathbb{Q}$, which satisfies the requirement of $x$ and $y$ being rational numbers.
Substituting these numbers into $x^y$ we get $2^{\frac{1}{2}} = \sqrt{2}$.
Based on our previous proofs we know that $\sqrt2$ is irrational.
Thus the statement "If $x$ and $y$ are rational numbers, then $x^y$ must be rational" is false.