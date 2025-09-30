## Problem 1

Prove that the following are equivalent for any subset $A$ and $B$ of the same universe $U$:

(a) $A \subseteq B$;

(b) $A \cap \overline{B} = \emptyset$;

(c) $\overline{A} \cup B = U$.

**-PF-**
We want to show that $a \implies b \implies c \implies a$.

($a \implies b)$: 
1. Assume $A \subseteq B$.
2. Suppose for contradiction that $A \cap \overline B \neq \emptyset$.
3. Then there exists some element $x$ such that $x \in A \cap \overline B$.
4. By definition of intersection, $x \in A$ and $x \in \overline B$.
5. Since $x \in \overline B$, by definition of the complement we know $x \not \in B$.
6. But since $A \subseteq B$ and $x \in A$, we must have $x \in B$.
7. This is a contradiction, as we now have $x \in B$ and $x \not \in B$.
8. Therefore our supposition was false and $A \cap \overline B = \emptyset$.

($b \implies c$):
1. Assume $A \cap \overline B = \emptyset$.
2. To show $\overline A \cup B = U$, we need to show $U \subseteq \overline A \cup B$ and $\overline A \cup B \subseteq U$.
3. $\overline A \cup B \subseteq U$ is automatic so we only need to prove $U \subseteq \overline A \cup B$.
4. Let $x$ be an arbitrary element of $U$.
5. Case 1: Suppose $x \in A$.
	- Since $A \cap \overline B = \emptyset$ and $x \in A$, we cannot have $x \in \overline B$.
	- Since $x \not \in \overline B$, $x \in B$.
	- Thus, $x \in \overline A \cup B$.
6. Case 2: Suppose $x \not \in A$.
	- Since $x \not \in A$, $x \in \overline A$.
	- Thus, $x \in \overline A \cup B$.
7. In all cases $x \in \overline A \cup B$.
8. Since $x$ was arbitrary, $U \subseteq \overline A \cup B$.
9. Therefore, $\overline A \cup B = U$.

($c \implies a$):
1. Assume $\overline A \cup B = U$.
2. Let $x$ be an arbitrary element of $A$.
3. Since $x \in A$ and $A \subseteq U$, we have $x \in U$.
4. Since $\overline A \cup B = U$, we know $x \in \overline A \cup B$.
5. By definition of union, $x \in \overline A$ or $x \in B$.
6. Since $x \in A$, $x \not \in \overline A$.
7. Therefore $x$ must be an element of $B$.
8. Since $x$ was arbitrary, every element of $A$ must be in $B$.
9. Therefore, $A \subseteq B$.

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