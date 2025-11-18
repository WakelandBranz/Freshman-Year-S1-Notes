### Problem 1

On the set $\mathbb{Z}$, let $R_1$ be the relation "divides" and let $R_2$ be the relation "is a multiple of". In other words $R_1 = {(a, b) \mid a|b}$ and $R_2 = {(a, b) \mid a = bk \text{ for some } k \in \mathbb{Z}}$. Find each of the following in as simple a description as possible.

**(a)** $R_1 \cap R_2$

$R_{1} \cap R_{2} = \{ (a, b) \mid |a| = |b| \}$

**(b)** $R_1 \cup R_2$

$R_1 \cup R_2 = \{ (a, b) \mid a \mid b \lor a = bk \text{ for some } k \in \mathbb{Z} \}$

**(c)** $R_2 - R_1$

---

### Problem 2

Let $R$ be a relation on $\mathbb{N} = {0, 1, 2, \cdots}$ that is both symmetric and transitive. Further, suppose that $(x, 7) \in R$ for all $x \in \mathbb{N}$. Show that $R$ induces a partition on $\mathbb{N}$.

---

### Problem 3

Let $S = \mathcal{P}({1, 2, 3, 4, 5})$. Define a relation $R$ on $S$ as follows: Set $A$ is related to set $B$ iff $|A| = |B|$.

**(a)** Determine the equivalence class $[{2, 3}]$.

$[\{2, 3\}] = \{ \{ 1, 2 \}, \{ 1, 3 \}, \{ 1, 4 \}, \{ 1, 5 \}, \{ 2, 3 \}, \{ 2, 4 \}, \{ 2, 5 \}, \{ 3, 4 \}, \{ 3, 5 \}, \{ 4, 5 \} \}$

**(b)** Determine the equivalence class $[\{\emptyset\}]$.

$[\{\emptyset\}] = \{\{ 1 \}, \{ 2 \}, \{ 3 \}, \{ 4 \}, \{ 5 \} \}$

**(c)** How many distinct equivalence classes does $R$ have? Explain your answer.

$R$ has 6 distinct equivalence classes. Since the cardinality of the largest set of $\mathcal{P}({1, 2, 3, 4, 5})$ is 5, and the power set includes the empty set, then there must be 6 distinct equivalence classes.

**(d)** How many distinct elements does each equivalence class contain?

$[\emptyset]$ contains 1 distinct element.
$[\{ 1 \}]$ contains 5 distinct elements.
$[\{ 1, 2 \}]$ contains 10 distinct elements.
$[\{ 1, 2, 3 \}]$ contains 6 distinct elements.
$[\{ 1, 2, 3, 4 \}]$ contains 3 distinct elements.
$[\{ 1, 2, 3, 4, 5 \}]$ contains 1 distinct element.

**(e)** Challenge/Ungraded: Come up with a formula to find the number of elements in each equivalence class so that we can be sure we do not miss any when doing a problem like part (d)?

Can you do the same thing for the same relation on the set $\mathcal{P}({1, 2, 3, \cdots, n})$?

---

### Problem 4

Given the relation $R$ on ${a, b, c, d}$ defined by the digraph below, determine, with justification, whether $R$ is symmetric, transitive, and/or reflexive. Provide explanation for each of the three properties.

**Digraph:**

- $a$ has edges to: $a$ (self-loop), $b$
- $b$ has edges to: $a$, $d$ (self-loop)
- $c$ has edges to: $c$ (self-loop), $a$
- $d$ has edges to: $d$ (self-loop), $b$

**Symmetric:**

**Transitive:**

**Reflexive:**

---

### Problem 5

Let $m > 1$ be an integer. Show that the relation $R$ on $\mathbb{Z}$ defined by $aRb$ if and only if $a \equiv b \pmod{m}$ is an equivalence relation.

---

### Problem 6

A relation $R$ is said to be **asymmetric** if $(a, b) \in R$ implies that $(b, a) \notin R$.

**(a)** If a relation is asymmetric, must it be antisymmetric? Prove your answer or provide a counterexample.

**(b)** If a relation is antisymmetric, must it be asymmetric? Prove your answer or provide a counterexample.