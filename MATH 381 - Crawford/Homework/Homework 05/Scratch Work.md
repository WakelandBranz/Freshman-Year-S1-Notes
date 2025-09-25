## Problem 1

Prove that the following are equivalent for any subset $A$ and $B$ of the same universe $U$:

(a) $A \subseteq B$;

(b) $A \cap \overline{B} = \emptyset$;

(c) $\overline{A} \cup B = U$.

**-PF (on the right track but wrong)-**
We want to show that $a \implies b \implies c \implies a$.
($a \implies b)$: 
	Assume $A \subseteq B$.
	Assume, for contradiction, that $A \cap \overline B \neq \emptyset$.
	This means that $A \subseteq B \implies \exists x \in A \cap \overline B$.
	But since $A \subseteq B$, all values of $A$ are contained within $B$.
	Since, by definition, if $x \in A$ and $x \not \in \overline B$, then $x \in B$.
	So, $\not \exists x$ such that $A$ is not in $B$, contradicting $x$'s existence.
	Thus $A \subseteq B \implies A \cap \overline B = \emptyset$.
($b \implies c$):
	Assume $A \cap \overline B$.
	Let $x \in U$.
	We want to show $x \in \overline A \cup B$.
	We can assume $x \not \in \overline A$, and show that $x \in B$. 
	===(Because if $x \in \overline A$, then $x \in \overline A \cup B$ which proves nothing).===
	
	
($c \implies a$):

**-PF- (he wrote this on the board)**
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

| $A$ | $B$ | $C$ | $B \cap C$ | $A \cup (B \cap C)$ | $B \cup C$ | $A \cap (B \cup C)$ |
| --- | --- | --- | ---------- | ------------------- | ---------- | ------------------- |
| 1   | 1   | 1   | 1          |                     |            |                     |
| 1   | 1   | 0   | 0          |                     |            |                     |
| 1   | 0   | 0   | 0          |                     |            |                     |
| 0   | 0   | 0   | 0          |                     |            |                     |
| 0   | 0   | 1   | 0          |                     |            |                     |
| 0   | 1   | 1   | 1          |                     |            |                     |
| 1   | 0   | 1   | 0          |                     |            |                     |
| 0   | 1   | 0   | 0          |                     |            |                     |

---
## Problem 4

For each $n \in \mathbb{Z}^+$, let $A_n = \left[\frac{1}{n}, 2 - \frac{n}{n+1}\right] \subset \mathbb{R}$. Find, and prove, the sets:

(a) $\bigcup_{n=1}^{\infty} A_n$;

(b) $\bigcap_{n=1}^{\infty} A_n$.

---
## Problem 5

Prove that if $A \subseteq B$, then $\mathcal{P}(A) \subseteq \mathcal{P}(B)$, where $\mathcal{P}(X)$ indicates the power set of the set $X$.

**-BAD PF-**
Assume that $A \subseteq B$.
Therefore, we know that all elements present in set $A$ are present in set $B$.
A power set contains every subset of the elements of an arbitrary set.
This means that if $A \subseteq B$, then $\mathcal{P}(B)$ will always contain the power set of $A$ because the contents of $A$ are present within $B$ thus every possible subset of $B$ includes every possible subset of $A$.
Thus, if $A \subseteq B$, then $\mathcal{P}(A) \subseteq \mathcal{P}(B)$.

**-PF-**
Assume $A \subseteq B$.
Let $S \in \mathcal{P}(A)$. 
We want to show $S \in \mathcal{P}(B$).
Since $S \in \mathcal{P}(A)$, we know that $S \subseteq A$.
Since $A \subseteq B$ and $S \subseteq A$, we know by hypothetical syllogism that $S \subseteq B$.
Therefore, $S \in \mathcal{P}(B)$.
Since our arbitrary element $S$ worked for this scenario, it must work for all elements of $\mathcal{P}(A)$.

---
## Problem 6

Define the symmetric difference of two sets $A$ and $B$, denoted $A \oplus B$, to be the set containing those elements in either $A$ or $B$, but not in both $A$ and $B$.

(a) Using the identities in Section 2.2, prove that $A \oplus B = (A - B) \cup (B - A)$.

(b) Sketch a Venn Diagram to represent $(A \oplus B) \cap B$.

(c) Prove or Disprove: $(A \oplus B) \cap B = B$.

---
## Problem 7

Write down all elements in the set $(A \times B) \times C$, where $A = \{1, 2, 3\}$, $B = \{4, 5 \}$ and $C = \{7, 8\}$.

$A \times B = \{ (1, 4), (1, 5), (1, 6), (2, 4), (2, 5), (2, 6), (3, 4), (3, 5), (3, 6) \}$
$$\begin{flalign}
(A \times B) \times C = \{ &((1, 4), 7), ((1, 4), 8), ((1, 5), 7), ((1, 5), 8), ((1, 6), 7), ((1, 6), 8), &\\
&((2, 4), 7), ((2, 4), 8), ((2, 5), 7), ((2, 5), 8), ((2, 6), 7), ((2, 6), 8), &\\
&((3, 4), 7), ((3, 4), 8), ((3, 5), 7), ((3, 5), 8), ((3, 6), 7), ((3, 6), 8) \} &
\end{flalign}$$