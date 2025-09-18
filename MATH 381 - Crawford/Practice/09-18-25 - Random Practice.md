##### Prove if $x$ is irrational, then $\frac{1}{x}$ is irrational.
**-PF-**
Towards contrapositive, we want to show if $\frac{1}{x}$ is rational, then $x$ is rational.
Assume $\frac{1}{x}$ is rational.
Then, $\exists a, b \in \mathbb{Z}$ such that $\frac{1}{x} = \frac{a}{b} \text{ and } b \neq 0$.
So, $\frac{1}{x} = \frac{a}{b} \equiv b = ax$.

##### Prove or disprove: There are irrational numbers $x$ and $y$ such that $x + y$ is rational.
**-PF-**
We want to show that there exist irrational numbers $x$ and $y$ such that $x + y$ is rational.
Towards an example, let $x = \sqrt{ 2 } \text{ and } y = -\sqrt{ 2 }$ meaning $x, y \not \in \mathbb{R}$.
So, substituting $x$ and $y$ into the expression $x + y$ we get $\sqrt{ 2 } - \sqrt{ 2 } = 0$.
Thus, since 0 is a rational number, this is proven.

##### Prove or disprove: 1 is the largest positive integer
**-PF-**
Let $n$ be the largest positive integer. ===- THIS HAS NOT BEEN PROVEN TO EXIST YET HENCE WHY THIS IS WRONG BUT THE ARGUMENT IS VALID!!!===
Then $n \geq 1$.
Since $n \geq 1$, multiply on both sides by $n, n^2 \geq n$.
But since $n$, by definition is the largest positive integer, $n \geq n^2 \implies n^2 = n$.
Then $n = 0$ or $n = 1$.
Since $n > 0 \implies n = 1$.

##### Prove if $x^2 \leq 1, \text{ then } x^2 -7x > -10$
**-PF-**
Assume $x^2 \leq 1$.
This means that $-1 \leq x \leq 1$.
$x^2 -7x > -10 \equiv x^2 -7x + 10 > 0$
$(x - 2)(x - 5) > 0 \equiv x^2 -7x + 10 > 0$.
In order for this statement to be true, $x > 5$ or $x < 2$.
Since $x^2 \leq 1 \equiv -1 \leq x \leq 1$, and $x^2 -7x > -10$ is true when $x < 2$, all cases of $x^2 -7x > -10$ are satisfied.
Thus if $x^2 \leq 1$ then $x^2 -7x > -10$.

##### Sudoku Problem
- Place the numbers 1-9 in each row, column, and 3x3 box so that there is only a single instance of each number in each row, column, and 3x3 box.
- **Prove**