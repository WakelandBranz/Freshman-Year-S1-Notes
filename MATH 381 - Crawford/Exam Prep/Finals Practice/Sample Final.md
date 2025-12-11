# Math 381: Discrete Mathematics Final Exam

## Table 1: Logical Equivalences

|Equivalence|Name|Expression|
|---|---|---|
|Identity laws|$p \land \mathbf{T}$|$\equiv p$|
||$p \lor \mathbf{F}$|$\equiv p$|
|Domination laws|$p \lor \mathbf{T}$|$\equiv \mathbf{T}$|
||$p \land \mathbf{F}$|$\equiv \mathbf{F}$|
|Idempotent laws|$p \lor p$|$\equiv p$|
||$p \land p$|$\equiv p$|
|Double negation law|$\neg(\neg p)$|$\equiv p$|
|Commutative laws|$p \lor q$|$\equiv q \lor p$|
||$p \land q$|$\equiv q \land p$|
|Associative laws|$(p \lor q) \lor r$|$\equiv p \lor (q \lor r)$|
||$(p \land q) \land r$|$\equiv p \land (q \land r)$|
|Distributive laws|$p \lor (q \land r)$|$\equiv (p \lor q) \land (p \lor r)$|
||$p \land (q \lor r)$|$\equiv (p \land q) \lor (p \land r)$|
|De Morgan's laws|$\neg(p \land q)$|$\equiv \neg p \lor \neg q$|
||$\neg(p \lor q)$|$\equiv \neg p \land \neg q$|
|Absorption laws|$p \lor (p \land q)$|$\equiv p$|
||$p \land (p \lor q)$|$\equiv p$|
|Negation laws|$p \lor \neg p$|$\equiv \mathbf{T}$|
||$p \land \neg p$|$\equiv \mathbf{F}$|
|Implication|$p \to q$|$\equiv \neg p \lor q$|
||$p \to q$|$\equiv \neg q \to \neg p$|
|Biconditional|$p \leftrightarrow q$|$\equiv (p \to q) \land (q \to p)$|
||$p \leftrightarrow q$|$\equiv q \leftrightarrow p$|
|Exclusive or|$p \oplus q$|$\equiv (p \lor q) \land \neg(p \land q)$|
||$p \oplus q$|$\equiv q \oplus p$|

---

## Table 2: Rules of Inference

|Rule of Inference|Tautology|
|---|---|
|Modus ponens|$(p \land (p \to q)) \to q$|
|Modus tollens|$(\neg q \land (p \to q)) \to \neg p$|
|Hypothetical syllogism|$((p \to q) \land (q \to r)) \to (p \to r)$|
|Disjunctive syllogism|$((p \lor q) \land \neg p) \to q$|
|Addition|$p \to (p \lor q)$|
|Simplification|$(p \land q) \to p$|
|Conjunction|$((p) \land (q)) \to (p \land q)$|
|Resolution|$((p \lor q) \land (\neg p \lor r)) \to (q \lor r)$|
|Universal instantiation|$(\forall x P(x)) \to P(c)$|
|Universal generalization|$(P(c) \text{ for arbitrary element } c) \to (\forall x P(x))$|
|Existential instantiation|$(\exists x P(x)) \to (P(c) \text{ for some element } c)$|
|Existential generalization|$(P(c) \text{ for some element } c) \to (\exists x P(x))$|

---

## Problem 1

Let $n$ be a positive integer. Show that $n^3 + 2n$ is divisible by 3.

_Hint: you can do it either by math induction or using modular arithmetic._

---

## Problem 2

1. Define the concept of _relatively prime_ integers $a$ and $b$.
    
2. Prove rigorously that 1937 and 2846 are relatively prime. Show all your work.
    

---

## Problem 3

Let $\mathbb{N} = {1, 2, 3, 4, \ldots}$ be the set of positive integers.

For each statement, select all equivalent logical statements.

---

**1.** A function $f: A \to B$ is _injective_.

(a) $\forall x \in A, \forall y \in A, (x = y) \to (f(x) = f(y))$

(b) $\forall x \in A, \forall y \in A, (f(x) \neq f(y)) \to (x \neq y)$

(c) $\forall x \in A, \forall y \in A, (f(x) = f(y)) \to (x = y)$

(d) $\forall x \in A, \forall y \in A, (x \neq y) \to (f(x) \neq f(y))$

---

**2.** A function $f: A \to B$ is _surjective_.

(a) $\forall x \in B, \exists y \in A, (f(y) = x)$

(b) $\forall y \in B, \exists x \in A, (f(x) = y)$

(c) $\forall y \in B, \exists y \in A, (f(y) = x)$

(d) $\forall x \in B, \exists y \in A, (f(x) = y)$

---

**3.** Integers $a$ and $b$ are _relatively prime_.

(a) $\forall d \in \mathbb{N}, ((d \mid a) \land (d = 1)) \to (d \mid b)$

(b) $\forall d \in \mathbb{N}, ((d \mid a) \land (d = 1)) \to (d \nmid b)$

(c) $\forall d \in \mathbb{N}, ((d \mid a) \land (d \neq 1)) \to (d \mid b)$

(d) $\forall d \in \mathbb{N}, ((d \mid a) \land (d \neq 1)) \to (d \nmid b)$

(e) $\forall d \in \mathbb{N}, ((d \mid a) \lor (d \mid b)) \to (d = 1)$

(f) $\forall d \in \mathbb{N}, ((d \mid a) \land (d \mid b)) \to (d \neq 1)$

(g) $\forall d \in \mathbb{N}, ((d \mid a) \lor (d \mid b)) \to (d \neq 1)$

(h) $\forall d \in \mathbb{N}, ((d \mid a) \land (d \mid b)) \to (d = 1)$

---

**4.** A positive integer $p > 1$ is prime.

(a) $\forall n \in \mathbb{N}, ((n \nmid p) \to (n \neq 1) \lor (n \neq p))$

(b) $\forall n \in \mathbb{N}, ((n \neq 1) \lor (n \neq p)) \to (n \nmid p)$

(c) $\forall n \in \mathbb{N}, ((n = 1) \land (n = p)) \to (n \mid p)$

(d) $\forall n \in \mathbb{N}, ((n \mid p) \to (n = 1) \land (n = p))$

(e) $\forall n \in \mathbb{N}, ((n \nmid p) \to (n \neq 1) \land (n \neq p))$

(f) $\forall n \in \mathbb{N}, ((n \neq 1) \land (n \neq p)) \to (n \nmid p)$

(g) $\forall n \in \mathbb{N}, ((n = 1) \lor (n = p)) \to (n \mid p)$

(h) $\forall n \in \mathbb{N}, ((n \mid p) \to (n = 1) \lor (n = p))$

---

## Problem 4

Given two sets $A$ and $B$ that are subsets of the universal set $U$, you have statements in the left column corresponding to properties or descriptions of these sets. Match each statement in the left column with its logically equivalent statement on the right side.

|Left Column||Right Column|
|---|---|---|
|1. $A \cap B = \emptyset$||A. $\exists x \in U ((x \in A) \leftrightarrow (x \in B))$|
|2. $A - B = \emptyset$||B. $\exists x \in U ((x \in A) \land \neg(x \in B))$|
|3. $U - A = B$||C. $\forall x \in U ((x \in A) \to (x \in B))$|
|4. $A \cup B = U$||D. $\forall x \in U ((x \in A) \lor (x \in B))$|
|5. $A \cap B \neq \emptyset$||E. $\forall x \in U ((\neg(x \in A)) \leftrightarrow (x \in B))$|
|6. $A - B \neq \emptyset$||F. $\forall x \in U ((\neg(x \in A)) \lor \neg(x \in B))$|
|7. $U - A \neq B$||G. $\exists x \in U ((\neg(x \in A)) \land \neg(x \in B))$|
|8. $A \cup B \neq U$||H. $\exists x \in U ((x \in A) \land (x \in B))$|

---

## Problem 5

Provide your answer as either a fraction or in decimal form.

1. You roll a fair six-sided die. Find the probability of rolling exactly a 2.
    
2. You roll two fair six-sided dice. Find the probability of rolling exactly an 8.
    
3. You roll three fair six-sided dice. Find the probability of rolling exactly a 10.
    

---

## Problem 6

Consider three relations $R_1, R_2, R_3$ on set $A = {a, b, c, d, e, f}$.

**1.**

(a) Relation $R_1$ is given as the following subset of $A \times A$: $$R_1 = {(a, b), (b, c), (c, a), (d, e), (e, f), (f, d)}$$ Represent $R_1$ as the direct graph and the matrix.

(b) Relation $R_2$ is given by the following directed graph:

_(Graph with vertices a, b, c, d, e, f and edges: e→d, d→b, f→a, f→c, a→c)_

Represent $R_2$ as the subset of $A \times A$ and the matrix.

(c) Relation $R_3$ is given by the following matrix:

||$a$|$b$|$c$|$d$|$e$|$f$|
|---|---|---|---|---|---|---|
|$a$|1|0|1|1|0|0|
|$b$|0|1|0|0|1|0|
|$c$|1|1|1|0|0|0|
|$d$|0|1|0|1|1|0|
|$e$|0|1|0|0|1|1|
|$f$|0|0|1|1|0|1|

Represent $R_3$ as the subset of $A \times A$ and the direct graph.

---

**2.** For each relation determine whether it is reflexive, symmetric, antisymmetric, transitive, or an equivalence relation. Fill the table with **T** for True and **F** for False.

||reflexive|symmetric|antisymmetric|transitive|equivalence relation|
|---|---|---|---|---|---|
|$R_1$||||||
|$R_2$||||||
|$R_3$||||||

---

## Problem 7

What is the coefficient of $x^8 y^{43}$ in the expansion of $(3x - 11y)^{51}$? Write the answer as a ratio of products of integers. You don't need to actually compute the final integer.

---

## Problem 8

Let $f: A \to B$ be a function. Recall the following definitions.

- If $S \subseteq A$, then $f[S] = {f(a) \mid a \in S}$ is the _image_ of $S$ under $f$.
- If $S \subseteq B$, then $f^{-1}[S] = {a \mid f(a) \in S}$ is the _preimage_ of $S$ under $f$.

**Note.** You **must not** use the inverse function $f^{-1}: B \to A$ because $f$ may be not invertible.

1. Give an example of a function $f: A \to B$ and $S, T \subseteq A$ such that $f[S] \cap f[T] \neq f[S \cap T]$.
    
2. Give an example of a function $f: A \to B$ and $S \subseteq A$ such that $S \neq f^{-1}[f[S]]$.
    
3. Give an example of a function $f: A \to B$ and $S \subseteq B$ such that $f[f^{-1}[S]] \neq S$.