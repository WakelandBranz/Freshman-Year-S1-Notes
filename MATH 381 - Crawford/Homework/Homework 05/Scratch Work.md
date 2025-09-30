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

**-PF-** ===he wrote this on the board===
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

Determine and prove the relationship between $X = A \cup (B \cap C)$ and $Y = A \cap (B \cup C)$, where $A,$ $B,$ and $C$ are any subset of the same universe $U$.

**-PF-**
Assume $A$, $B$, and $C$, are any subset of the same universe $U$.
We will use a membership table to determine a relationship between $X$ and $Y$.

| $A$ | $B$ | $C$ | $B \cap C$ | $(X) \text{ }A \cup (B \cap C)$ | $B \cup C$ | $A \cap (B \cup C)$ |
| --- | --- | --- | ---------- | ------------------------------- | ---------- | ------------------- |
| 1   | 1   | 1   | 1          | 1                               | 1          | 1                   |
| 1   | 1   | 0   | 0          | 1                               | 1          | 1                   |
| 1   | 0   | 0   | 0          | 1                               | 0          | 0                   |
| 0   | 0   | 0   | 0          | 0                               | 0          | 0                   |
| 0   | 0   | 1   | 0          | 0                               | 1          | 0                   |
| 0   | 1   | 1   | 1          | 1                               | 1          | 0                   |
| 1   | 0   | 1   | 0          | 1                               | 1          | 1                   |
| 0   | 1   | 0   | 0          | 0                               | 1          | 0                   |

Using the membership table above, we can see that every time $Y$ is 1, $X$ is also 1, but it is not true that every time $X$ is 1, $Y$ is also 1.
By the definition of a proper subset, we can see that $Y \subseteq X$ but $Y \neq X$.
Therefore, the relationship between $X$ and $Y$ is that $Y$ is a proper subset of $X$.

---
## Problem 4

For each $n \in \mathbb{Z}^+$, let $A_n = \left[\frac{1}{n}, 2 - \frac{n}{n+1}\right] \subset \mathbb{R}$. Find, and prove, the sets:

(a) $\bigcup_{n=1}^{\infty} A_n$;
$[\frac{1}{1}, 2 - \frac{1}{2}], [\frac{1}{2}, 2 - \frac{2}{3}], [\frac{1}{3}, 2 - \frac{3}{4}], [\frac{1}{4}, 2 - \frac{4}{5}]$
$\bigcup_{n=1}^{\infty} A_n = \{ (0, \frac{3}{2}] \}$ 

**-PF-**
$A_{n}$ approaches but never reaches 0 since $\frac{1}{n}$ decreases for every subsequent $n$.
$A_{n}$ reaches its greatest value, $\frac{3}{2}$ when $n = 1$.
Thus, $\bigcup_{n=1}^{\infty} A_n = \{ (0, \frac{3}{2}] \}$.

(b) $\bigcap_{n=1}^{\infty} A_n$.
$[\frac{1}{1}, 2 - \frac{1}{2}], [\frac{1}{2}, 2 - \frac{2}{3}], [\frac{1}{3}, 2 - \frac{3}{4}], [\frac{1}{4}, 2 - \frac{4}{5}]$
$\bigcap_{n=1}^{\infty} A_n = \{1\}$.

**-PF-**
First, we simplify the right endpoint: $2 - \frac{n}{n+1} = 1 + \frac{1}{n+1}$.
So $A_n = \left[\frac{1}{n}, 1 + \frac{1}{n+1}\right]$.
The value $1$ is in every $A_n$ since $\frac{1}{n} \leq 1 \leq 1 + \frac{1}{n+1}$ for all $n \geq 1$.
Now consider any $x \neq 1$. 
If $x < 1$, then as $n$ increases, $\frac{1}{n}$ eventually becomes larger than $x$, so $x$ is not in $A_n$ for large enough $n$. 
Similarly, if $x > 1$, then $1 + \frac{1}{n+1}$ eventually becomes smaller than $x$, so $x$ is not in $A_n$ for large enough $n$.
Since only $1$ belongs to every $A_n$, we have $\bigcap_{n=1}^{\infty} A_n = {1}$.

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

#### (a) Using the identities in Section 2.2, prove that $A \oplus B = (A - B) \cup (B - A)$

**-OLD PF-**
By the set difference definition, $(A - B) = \{x \mid x \in A \land x \not \in B \}$.
So, we can rewrite our equation as $\{ x \mid x \in A \land x \not \in B \} \cup (B - A)$.
By the set difference definition, $(B - A) = \{ x \mid x \in B \land x \not \in A \}$.
So, we can rewrite our equation as $\{ x \mid x \in A \land x \not \in B \} \cup \{ x \mid x \in B \land x \not \in A \}$.
This tells us that the set $(A - B) \cup (B - A)$ is all elements $x$ such that $\exists x \in A \land x \not \in B$ or $\exists x \in B \land x \not \in A$.

**-PF-**
From the definition, $A \oplus B = (A \cup B) - (A \cap B)$.
Applying the definition of set differences we get $(A \cup B) - (A \cap B) = (A \cup B) \cap \overline{(A \cap B)}$.
Applying DeMorgan's Law, we get $(A \cup B) \cap \overline{(A \cap B)} = (A \cup B) \cap (\overline A \cup \overline B)$.
Applying the Distributive Law, we get $(A \cup B) \cap (\overline A \cup \overline B) = ((A \cup B) \cap \overline A) \cup ((A \cup B) \cap \overline B)$.
Applying the Associative Law to each side of the equation we get $(\overline A \cap (A \cup B)) \cup (\overline B \cap (A \cup B))$.
Applying the Distributive Law to the left side of the equation we get the following: $(\overline A \cap (A \cup B)) = (\overline A \cap A) \cup (\overline A \cap B)$.
By the Complement Law, $(\overline A \cap A) \cup (\overline A \cap B) = \emptyset \cup (\overline A \cap B)$.
By the Identity Law, $\emptyset \cup (\overline A \cap B) = \overline A \cap B$.
By the Commutative Law $\overline A \cap B = B \cap \overline A$.
By the definition of set differences, $B \cap \overline A = B - A$.
Applying the Distributive Law to the right side of the equation we get the following: $(\overline B \cap (A \cup B)) = (\overline B \cap A) \cup (\overline B \cap B)$.
By the Complement Law, $(\overline B \cap A) \cup (\overline B \cap B) = (\overline B \cap A) \cup \emptyset$.
By the Identity Law, $(\overline B \cap A) \cup \emptyset = \overline B \cap A$.
By the Commutative Law, $\overline B \cap A = A \cap \overline B$.
By the definition of set differences, $A \cap \overline B = A - B$.
So, $A \oplus B = (B - A) \cup (A - B)$.
By the Commutative Law, $(B - A) \cup (A - B) = (A - B) \cup (B - A)$.
So, $A \oplus B = (A \cup B) - (A \cap B) = (A - B) \cup (B - A)$, thus proving that they are equivalent.

---

#### (b) Sketch a Venn Diagram to represent $(A \oplus B) \cap B$.

[thing](obsidian://open?vault=UNC-FreshmanS1Notes&file=MATH%20381%20-%20Crawford%2FImages%2FVenn%20Diagram%202.1%20%26%202.2%20Problem%206%20Part%20B)
![[Homework 2.1 & 2.2 Venn Diagram.png]]
---

#### (c) Prove or Disprove: $(A \oplus B) \cap B = B$.

**-PF-**
We will use a membership table to disprove the statement $(A \oplus B) \cap B = B$.

| $A$ | $B$ | $A \oplus B$ | $(A \oplus B) \cap B$ |
| --- | --- | ------------ | --------------------- |
| 1   | 1   | 0            | 0                     |
| 1   | 0   | 1            | 0                     |
| 0   | 1   | 1            | 1                     |
| 0   | 0   | 0            | 0                     |
Using the membership table above, we can see that when $B$ is 1, $(A \oplus B) \cap B$ is not always 1.
This can be seen in row 1, where $B = 1$ and $(A \oplus B) \cap B = 0$.
Therefore, $(A \oplus B) \cap B = B$ is false.

---
## Problem 7

Write down all elements in the set $(A \times B) \times C$, where $A = \{1, 2, 3\}$, $B = \{4, 5 \}$ and $C = \{7, 8\}$.

$A \times B = \{ (1, 4), (1, 5), (1, 6), (2, 4), (2, 5), (2, 6), (3, 4), (3, 5), (3, 6) \}$
$$\begin{flalign}
(A \times B) \times C = \{ &((1, 4), 7), ((1, 4), 8), ((1, 5), 7), ((1, 5), 8), ((1, 6), 7), ((1, 6), 8), &\\
&((2, 4), 7), ((2, 4), 8), ((2, 5), 7), ((2, 5), 8), ((2, 6), 7), ((2, 6), 8), &\\
&((3, 4), 7), ((3, 4), 8), ((3, 5), 7), ((3, 5), 8), ((3, 6), 7), ((3, 6), 8) \} &
\end{flalign}$$