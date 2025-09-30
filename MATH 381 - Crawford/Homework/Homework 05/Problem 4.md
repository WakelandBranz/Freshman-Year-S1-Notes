***(a)***
**-PF-**
Let $x \in (-\infty, 0] \cup (\frac{3}{2}, \infty)$.
We want to show that $x \not \in \bigcup^\infty_{n = 1} A_{n}.$
Since $x \in (-\infty, 0] \cup (\frac{3}{2}, \infty)$, $x \not \in A_n$ for every $n$.
So, $x \not \in [  \frac{1}{n}, 1 + \frac{1}{n + 1} ]$ for every $n$.
So, $x < \frac{1}{n}$ or $x > 1 + \frac{1}{n + 1}$ for every $n$.
Since $0 < \frac{1}{n} \space \forall n$, $\{ x \mid x \leq 0 \}$ satisfies $x < \frac{1}{n} \forall n$.
For $x > \frac{3}{2} = 1 + \frac{1}{2} = 1 + \frac{1}{1 + 1}$, so $x \not \in A_n$ for $\forall n$.
For any $x \in (-\infty, 0] \cup (\frac{3}{2}, \infty), \space x \not \in \bigcup^\infty_{n=1} A_n.$
So, $\bigcup^\infty_{n=1} A_n \subseteq (0, \frac{3}{2}]$.
We want to show $(0, \frac{3}{2}] \subseteq \bigcup^\infty_{n=1} A_n.$
Case 1: $x \in [1, \frac{3}{2}].$
	If $x \in [1, \frac{3}{2}]$ then $x \in A_1$ then $x \in \bigcup^\infty_{n=1} A_n$.
Case 2: $x \in (0, 1)$.
	Let $x \in (0, 1)$.
	Let $n \in \mathbb{Z^+}$ be such that $n > \frac{1}{x} \rightarrow x > \frac{1}{n}$.
	Then $x \in A_n$.
***(b)***
**-PF-**
Let $x \in \bigcup^\infty_{n=1} A_n$.
So, $x \in A_n \forall n$.
So, $\frac{1}{n} \leq x \leq 1 + \frac{1}{n + 1} \forall n$