# Homework 2.3 - Wakeland Branz

## 1. Characteristic Function

For a universal set $U$ and a subset $A \subseteq U$, we define the characteristic function of $A$, written as $\chi_A : U \to {0, 1}$, to be the function

$$\chi_A(x) = \begin{cases} 1 & \text{if } x \in A \ 0 & \text{if } x \notin A \end{cases}$$

**(a)** If $A = [0, 2) \subset \mathbb{R}$, sketch the graph of $\chi_A$.

**(b)** If $A = [0, 2) \subset \mathbb{R}$, determine $\chi_A^{-1}(0)$, $\chi_A^{-1}(1)$, and $\chi_A^{-1}(2)$.

---

## 2. Injective/Surjective Functions from $\mathbb{Z}$ to $\mathbb{Z}$

Determine, with proof, if the following functions from $\mathbb{Z}$ to $\mathbb{Z}$ are injective/surjective.

**(a)** $f(n) = n^2 + 1$

WTS that $f(n) = n^2 + 1$ is neither injective nor surjective.
To prove that  from  is not injective, we can use a counterexample.
Take two cases.
Case 1: $n = -1$
Since $n = -1$, $f(-1) = (-1)^2 + 1 = 2$.
Case 2: $n = 1$
Since $n = 1, f(1) = 1^2 + 1 = 2$.
Since $f(1) = f(-1) = 2$, $n^2 + 1$ is not injective.
To prove that $f(n)$ from $\mathbb{Z} \rightarrow \mathbb{Z}$ is not surjective, we can use a counterexample where $n^2 + 1 = 3$.
So, $n^2 + 1 = 3 \rightarrow n^2 = 2 \rightarrow n = \sqrt{ 2 }$.
Since $\sqrt 2 \not \in \mathbb{Z}$ and there is no integer $n$ such that $f(n) = 3$, $n^2 + 1$ cannot be surjective.


**(b)** $f(n) = n^3$

Injective

**(c)** $f(n) = \lceil \frac{n}{2} \rceil$ where $\lceil x \rceil$ denotes the smallest integer greater than or equal to $x$.

Neither injective **nor** surjective

---

## 3. Injective/Surjective Functions from $\mathbb{Z} \times \mathbb{Z}$ to $\mathbb{Z}$

Determine, with proof, if the following functions from $\mathbb{Z} \times \mathbb{Z}$ to $\mathbb{Z}$ are injective/surjective.

**(a)** $f(m, n) = 2m - n$

Assume, for contradiction, that $f(m, n) = 2m - n \text{ from } \mathbb{Z} \text{ x } \mathbb{Z} \text{ to } \mathbb{Z}$ is injective.
For counterexample, we have two cases.
Case 1: $m = 2, n = 4 \rightarrow f(2, 4) = 2(2) - 4 = 0$.
Case 2: $m = 1, n = 2 \rightarrow f(1, 2) = 2(1) - 2 = 0$.
But since these two cases have different preimages resulting in the same image, this is a contradiction.
Thus $f(m, n) = 2m - n$ is not injective.

WTS that $f(m, n) = 2m - n$ is surjective. 
Let $y \in \mathbb{Z}$ be arbitrary.
We want to find $m, n \in \mathbb{Z}$ s.t. $f(m, n) = y$.
We need $f(m, n) = 2m - n = y$.
Let $m = 0, n = -y$.
So, $f(m, n) = 2(0) - (-y) = y$.
Since there is a case where $f(m, n) = y$ and $y \in \mathbb{Z}$ and $y$ is an arbitrary number, $f(m, n)$ is surjective.

**(b)** $f(m, n) = m^2 - n^2$

Assume, for contradiction, that $f(m, n) = m^2 - n^2 \text{ from } \mathbb{Z} \text{ x } \mathbb{Z} \text{ to } \mathbb{Z}$ is injective.
For counterexample, we have two cases.
Case 1: $m = 2, n = 2 \rightarrow f(2, 4) = 2^2 - 2^2 = 0$.
Case 2: $m = 1, n = 1 \rightarrow f(1, 1) = 1^2 - 1^2 = 0$.
But since these two cases have different preimages resulting in the same image, this is a contradiction.
Thus $f(m, n) = m^2 - n^2$ is not injective.

WTS that $f(m, n)$ is not surjective.
Assume, for contradiction, that $f(m, n)$ is surjective.
Suppose there exists $y \in \mathbb{Z}$ s.t. $f(m, n) = 2$.
So, $m^2 - n^2 = 2 \rightarrow (m + n)(m - n) = 2$.
There are 4 cases where this statement will hold true.
Case 1: 

**(c)** $f(m, n) = |m| - |n|$

Assume, for contradiction, that $f(m, n) = |m| - |n| \text{ from } \mathbb{Z} \text{ x } \mathbb{Z} \text{ to } \mathbb{Z}$ is injective.
For counterexample, we have two cases.
Case 1: $m = 2, n = 2 \rightarrow f(2, 4) = |2| - |2| = 0$.
Case 2: $m = -2, n = -2 \rightarrow f(1, 2) = |-2| - |-2| = 0$.
But since these two cases have different preimages resulting in the same image, this is a contradiction.
Thus $f(m, n) = |m| - |n|$ is not injective.

---

## 4. Examples of Functions from $\mathbb{N}$ to $\mathbb{N}$

Give an example of a function from $\mathbb{N}$ to $\mathbb{N}$ that is

**(a)** injective, but not surjective;

$f(n) = n + 1$

---

**(b)** surjective, but not injective;

$$f(n) = \begin{cases} 
   0 & \text{if } n < 2
\\ n - 1 & \text{if } n \geq 2 
\end{cases}$$

---

**(c)** both injective and surjective, but is not equal to the identity function;

$$f(n) = \begin{cases} 
   1 & \text{if } n = 0
\\ 0 & \text{if } n = 1
\\ n & \text{if } n \geq 2 
\end{cases}$$

---

**(d)** is neither injective nor surjective.

$$f(n) = \begin{cases} 
   0 & \text{if } n < 3
\\ n^2 & \text{if } n \geq 3 
\end{cases}$$

---

## 5. Function Composition Properties

Suppose $g : A \to B$ and $f : B \to C$ are functions. Prove

**(a)** If $f \circ g$ is surjective, then $f$ must also be.

WTS that if $f \circ g$ is surjective, then $f$ is also surjective.
Assume $f \circ g$ is surjective.
Since $g: A \rightarrow B$ and $f: B \rightarrow C$, $f \circ g: A \rightarrow C$.
From this we know that $f$'s codomain equals $f \circ g$'s codomain.
By definition, since $f \circ g$ is surjective, $\forall c \in C, \exists a \in A$ such that $f(g(a)) = c$.


**(b)** If $f \circ g$ is injective, then $g$ must also be.

**(c)** If $f \circ g$ is a bijection, then $g$ is surjective if and only if $f$ is injective.

**(d)** Give an example where $f \circ g$ is surjective, but $g$ is not.

---

## 6. Images of Sets Under Functions

Let $f : A \to B$ be a function and $S, T \subseteq A$. Prove that

**(a)** $f(S \cup T) = f(S) \cup f(T)$

**(b)** $f(S \cap T) \subseteq f(S) \cap f(T)$, but equality need not hold in general.

---

## 7. Inverse Images of Sets

Let $f : A \to B$ be a function. Define the inverse image of $S \subseteq B$ to be the set

$$f^{-1}(S) = {a \in A \mid f(a) \in S}$$

Note that this can be defined whether or not $f$ is an invertible function.

Prove that for subsets $S, T \subseteq B$, $f^{-1}(S \cup T) = f^{-1}(S) \cup f^{-1}(T)$.