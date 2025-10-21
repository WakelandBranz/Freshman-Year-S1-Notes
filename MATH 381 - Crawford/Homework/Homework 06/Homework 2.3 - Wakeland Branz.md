## 1. Characteristic Function

For a universal set $U$ and a subset $A \subseteq U$, we define the characteristic function of $A$, written as $\chi_A : U \to {0, 1}$, to be the function

$$\chi_A(x) = \begin{cases} 1 & \text{if } x \in A \ 0 & \text{if } x \notin A \end{cases}$$

**(a)** If $A = [0, 2) \subset \mathbb{R}$, sketch the graph of $\chi_A$.

**(b)** If $A = [0, 2) \subset \mathbb{R}$, determine $\chi_A^{-1}(0)$, $\chi_A^{-1}(1)$, and $\chi_A^{-1}(2)$.

---

## 2. Injective/Surjective Functions from $\mathbb{Z}$ to $\mathbb{Z}$

Determine, with proof, if the following functions from $\mathbb{Z}$ to $\mathbb{Z}$ are injective/surjective.

**(a)** $f(n) = n^2 + 1$

**(b)** $f(n) = n^3$

**(c)** $f(n) = \lceil \frac{n}{2} \rceil$ where $\lceil x \rceil$ denotes the smallest integer greater than or equal to $x$.

---

## 3. Injective/Surjective Functions from $\mathbb{Z} \times \mathbb{Z}$ to $\mathbb{Z}$

Determine, with proof, if the following functions from $\mathbb{Z} \times \mathbb{Z}$ to $\mathbb{Z}$ are injective/surjective.

**(a)** $f(m, n) = 2m - n$

**(b)** $f(m, n) = m^2 - n^2$

**(c)** $f(m, n) = |m| - |n|$

---

## 4. Examples of Functions from $\mathbb{N}$ to $\mathbb{N}$

Give an example of a function from $\mathbb{N}$ to $\mathbb{N}$ that is

**Note, my definition of $\mathbb{N}$ includes 0**

**(a)** injective, but not surjective;

$f(n) = n + 1$

**(b)** surjective, but not injective;

$f(n) = $

**(c)** both injective and surjective, but is not equal to the identity function;

$f(n) = $

**(d)** is neither injective nor surjective.

---

## 5. Function Composition Properties

Suppose $g : A \to B$ and $f : B \to C$ are functions. Prove

**(a)** If $f \circ g$ is surjective, then $f$ must also be.

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

Let $x \in f^{-1}(S \cup T)$ be arbitrary.
By the definition of inverse functions, $f^{-1}(S \cup T)$ is the set of numbers which map to the preimage of $S \cup T$.
Therefore, $x$ is in the preimage of $S \cup T$.
