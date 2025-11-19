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

In order for $R$ to induce a partition on $\mathbb{N}$, $R$ must produce equivalence classes which, when summed, are equivalent to $\mathbb{N}$.

---

### Problem 3

Let $S = \mathcal{P}(\{1, 2, 3, 4, 5\})$. Define a relation $R$ on $S$ as follows: Set $A$ is related to set $B$ iff $|A| = |B|$.

**(a)** Determine the equivalence class $[\{2, 3\}]$.

$[\{2, 3\}] = \{ \{ 1, 2 \}, \{ 1, 3 \}, \{ 1, 4 \}, \{ 1, 5 \}, \{ 2, 3 \}, \{ 2, 4 \}, \{ 2, 5 \}, \{ 3, 4 \}, \{ 3, 5 \}, \{ 4, 5 \} \}$

**(b)** Determine the equivalence class $[\{\emptyset\}]$.

This question doesn't make sense.
The power set $\mathcal{P}({1, 2, 3, 4, 5})$ does not contain an element $\{ \emptyset \}$ thus this is an invalid equivalence class.

**(c)** How many distinct equivalence classes does $R$ have? Explain your answer.

$R$ has 6 distinct equivalence classes. Since the cardinality of the largest set of $\mathcal{P}({1, 2, 3, 4, 5})$ is 5, and the power set includes the empty set, then there must be 6 distinct equivalence classes.

**(d)** How many distinct elements does each equivalence class contain?

$[\emptyset]$ contains 1 distinct element.
$[\{ 1 \}]$ contains 5 distinct elements.
$[\{ 1, 2 \}]$ contains 10 distinct elements.
$[\{ 1, 2, 3 \}]$ contains 10 distinct elements.
$[\{ 1, 2, 3, 4 \}]$ contains 5 distinct elements.
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

Relation: $\{ a, b \in \mathbb{Z} \times \mathbb{Z} \mid a \equiv b \pmod{m}  \}$

Reflexive:

Let $a \in \mathbb{Z}$ be arbitrary. WTS $aRa$.
By the definition of $R$, we need to show $a \equiv a \pmod{m}$.
By the definition of congruence modulo $m$, we need to show $m \mid (a - a)$.
Since $a - a = 0$ and $0 = m \cdot 0$, we have $m \mid (a - a)$.
Therefore $a \equiv a \pmod{m}$ which tells us $aRa$.
Since $a$ was arbitrary, $R$ is reflexive.

Symmetric:

Let $a, b \in \mathbb{Z}$ be arbitrary. 
Assume $aRb$. WTS $bRa$.
By the definition of $R$, we have $a \equiv b \pmod{m}$.
By the definition of congruence, $m \mid (a - b)$.
By the definition of divisibility, $a - b = mn$ for some integer $n$.
Multiplying the entire equivalence $a - b = mn$ by $-1$ gives us $b - a = m(-n)$.
Since $-n \in \mathbb{Z}$, we have $m \mid (b - a) \to b \equiv a \pmod{m}$.
Thus $bRa$.
Since $a, b$ were arbitrary, $R$ is symmetrical.

Transitive:

Let $a, b, c \in \mathbb{Z}$ be arbitrary.
Assume $aRb$ and $bRc$. WTS $aRc$.
By the definition of $R$, we have $a \equiv b \pmod{m}$ and $b \equiv c \pmod{m}$.
By the definition of congruence, $m \mid (a - b)$ and $m \mid (b - c)$.
By the definition of divisibility, $a - b = mn_1$ and $b - c = mn_2$ for integers $n_1, n_2$. 
Isolate $b$ in the equality $a - b = mn_1$ to get $b = -mn_1 + a$.
Substitute this $b$ into $b - c = mn_2$ to get $(-mn_1 + a) - c = mn_2$.
This simplifies to $a - c = mn_1 + mn_2 \to a - c = m(n_1 + n_2)$.
Since $(n_1 + n_2) \in \mathbb{Z}$, we have $m \mid (a - c)$.
Therefore, $a \equiv c \pmod{m}$ and $aRc$.

So, relation $R$ is an equivalence relation.

---

### Problem 6

A relation $R$ is said to be **asymmetric** if $(a, b) \in R$ implies that $(b, a) \notin R$.

**(a)** If a relation is asymmetric, must it be antisymmetric? Prove your answer or provide a counterexample.

By the definition of an antisymmetric relation, if $(a, b) \in R$ and $(b, a) \in R$, then $a = b$.
If a relation is asymmetric, then $(b, a) \not \in R$, so the hypothesis of an antisymmetric relation is always false. 
Thus, since the hypothesis of the definition of antisymmetric is always false in asymmetric relations, an asymmetric relation is always antisymmetric.

**(b)** If a relation is antisymmetric, must it be asymmetric? Prove your answer or provide a counterexample.

Take two cases:

Case 1: Assume a relation is antisymmetric because the hypothesis and conclusion of the definition of antisymmetry are true.
By the definition of an antisymmetric relation, if $(a, b) \in R$ and $(b, a) \in R$, then $a = b$.
By the definition of asymmetric, the hypothesis $(a, b) \in R$ is always true because all antisymmetric relations have $(a, b) \in R$.
By the definition of asymmetric, the conclusion $(b, a) \not \in R$ is always false because all antisymmetric relations have $(b, a) \in R$.
In antisymmetric relations, the asymmetric property's hypothesis is true and the conclusion is false.
Therefore no antisymmetric relation is asymmetric when the hypothesis and conclusion of the definition of antisymmetry are true.

Case 2: Assume a relation is antisymmetric because the hypothesis of the definition of antisymmetry is false.
This means that the conclusion of the definition of antisymmetry can be either false or true, thus $(a, b) \in R$ or $(a, b) \not \in R$.

