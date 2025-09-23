## Problem 1

Prove that the following are equivalent for any subset $A$ and $B$ of the same universe $U$:

(a) $A \subseteq B$;

(b) $A \cap \overline{B} = \emptyset$;

(c) $\overline{A} \cup B = U$.

**-PF-**
We want to show that $a \implies b \implies c \implies a$.
($a \implies b)$: 
	Assume $A \subseteq B$.
	Assume, for contradiction, that $A \cap \overline B \neq \emptyset$.
	This means that $A \subseteq B \implies \exists x \in A \cap \overline B$.
	But since $A \subseteq B$, all values of $A$ are contained within $B$.
	So, $\not \exists x$ such that $A$ is not in $B$, contradicting $x$'s existence.
	Thus $A \subseteq B \implies A \cap \overline B = \emptyset$.
($b \implies c$):

($c \implies a$):

**-PF-**
We want to show that $a \implies b \implies c \implies a$.
($a \implies b)$: 
	Assume that $A \subseteq B$. 
	We want to show that $A \cap \overline B = \emptyset$.
	We show containment both ways.
	We wrote $\emptyset \subseteq A \cap \overline B$ since $\emptyset$ is a subset of every set.
	To show $A \cap \overline B \subseteq \emptyset$, it suffices to show there does not exist any element in $A \cap \overline B$.
	Assume $x \in A \cap \overline B$, then $x \in \{ y \mid y \in A \cap y \not \in B \}$.
	But since $A \subseteq B$, there are no elements in $A$ and not in $B$. 
	This contradicts $x$'s existence.
	So $x$ cannot exist. 
	So $A \cap \overline B \subseteq \emptyset \implies A \cap \overline B = \emptyset$.
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