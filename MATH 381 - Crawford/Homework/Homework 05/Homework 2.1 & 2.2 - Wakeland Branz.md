## Problem 1

Prove that the following are equivalent for any subset $A$ and $B$ of the same universe $U$:

(a) $A \subseteq B$;

(b) $A \cap \overline{B} = \emptyset$;

(c) $\overline{A} \cup B = U$.

**-PF-**
We want to show that $a \implies b \implies c \implies a$.
($a \implies b)$: 
	(a) = $A \subseteq B$ which means that all elements of $A$ are present in $B$ or all elements of $B$ are in $A$. 
	(b) = $A \cap \overline B = \emptyset$ which means that there are no intersections between $A$ and $\overline B$. 
	We assume that if $A \subseteq B$ then $A \cap \overline B = \emptyset$.
	This means that since $A$ is contained within $B$, there are no intersections between $A$ and everything that is not contained within $B$.
($b \implies c$):
($c \implies a$):

**-PF-**
We want to show that $a \implies b \implies c \implies a$.
($a \implies b)$: 
($b \implies c$):
($c \implies a$):

---
## Problem 2

Prove or disprove: For any sets $A$, $B$, and $C$, if $A \cup B = A \cup C$, then $B = C$.

**-PF-**
We will assume that for any sets $A$, $B$, and $C$, if $A \cup B = A \cup C$, then $B = C$.
We will disprove this using a counterexample.
Let $A = \{ 1, 2, 3, 4 \}$, $B = \{ 2, 3 \}$, and $C = \{ 3, 4 \}$.
In this case, $A \cup B = \{ 1, 2, 3, 4 \}$ and $A \cup C = \{ 1, 2, 3, 4 \}$.
Despite the fact that $A \cup B = A \cup C$, $B$ and $C$ are not equivalent.
Thus we disprove that, for any sets $A$, $B$, and $C$, if $A \cup B = A \cup C$, then $B = C$.

---
## Problem 3

Determine and prove the relationship between $X = A \cup (B \cap C)$ and $Y = A \cap (B \cup C)$, where $A$, $B$, and $C$ are any subset of the same universe $U$.

---
## Problem 4

For each $n \in \mathbb{Z}^+$, let $A_n = \left[\frac{1}{n}, 2 - \frac{n}{n+1}\right] \subset \mathbb{R}$. Find, and prove, the sets:

(a) $\bigcup_{n=1}^{\infty} A_n$;

(b) $\bigcap_{n=1}^{\infty} A_n$.

---
## Problem 5

Prove that if $A \subseteq B$, then $\mathcal{P}(A) \subseteq \mathcal{P}(B)$, where $\mathcal{P}(X)$ indicates the power set of the set $X$.

---
## Problem 6

Define the symmetric difference of two sets $A$ and $B$, denoted $A \oplus B$, to be the set containing those elements in either $A$ or $B$, but not in both $A$ and $B$.

(a) Using the identities in Section 2.2, prove that $A \oplus B = (A - B) \cup (B - A)$.

(b) Sketch a Venn Diagram to represent $(A \oplus B) \cap B$.

(c) Prove or Disprove: $(A \oplus B) \cap B = B$.

---
## Problem 7

Write down all elements in the set $(A \times B) \times C$, where $A = {1, 2, 3}$, $B = {4, 5, 6}$ and $C = {7, 8}$.