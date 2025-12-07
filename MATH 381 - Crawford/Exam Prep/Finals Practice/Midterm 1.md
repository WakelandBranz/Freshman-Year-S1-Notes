# Math 381 Test 1 Fall 2025

**October 2, 2025**

---

**1.** (3 points) Let $T(x, y)$ be the statement "$x$ teaches $y$", where the domain of $x$ consists of all teachers at UNC and the domain of $y$ is all classes at UNC. Translate the following statement into propositional logic without using $\exists!$.

"Ramses teaches exactly one class at UNC."

A. $\forall x \exists y , (T(x, y) \land \forall z (z \neq y \rightarrow T(x, z)))$

B. $\exists x \forall y , (T(x, y) \land \forall z (z \neq y \rightarrow T(x, z)))$

C. $\forall y , (T(\text{Ramses}, y) \land \exists z (z \neq y \rightarrow \neg T(\text{Ramses}, z)))$

D. $\exists y , (T(\text{Ramses}, y) \land \forall z (z \neq y \rightarrow \neg T(\text{Ramses}, z)))$

---

**2.** True/False. Determine the truth values of the following statements. If True, no justification is needed. If False, provide a counterexample.

(a) (1 point) $\exists x \in \mathbb{Z} ; \forall y \in \mathbb{Z} ; \left( y \neq 0 \rightarrow \frac{x}{y} = 0 \right)$

(b) (1 point) $\exists x \in \mathbb{Q} ; \exists y \in \mathbb{Q} ; (\sqrt{x} = y)$

(c) (1 point) $\forall x \in \mathbb{R} ; \forall y \in \mathbb{R} ; (xy > 0 \rightarrow (x > 0 \land y > 0))$

(d) (1 point) $\forall n \in \mathbb{Z} ; (n < n^2)$

---

**3.** The following is a supposed proof that 1 is the largest positive integer.

"Let $n$ be the largest positive integer. Then $n \geq 1$. Therefore, multiplying both sides by $n$, we have $n^2 \geq n$. But since $n$ is the largest positive integer, it must be that $n^2 \leq n$. Hence $n^2 \geq n$ and $n^2 \leq n$, implying $n^2 = n$. Dividing both sides by $n$, we see that $n = 1$."

(a) (1 point) Is this a **valid** or **invalid** argument? (Circle one.)

(b) (2 points) Which of these statements is most correct?

A. The statement "Let $n$ be the largest positive integer." is a False premise.

B. The statement "If $n \geq 1$, then $n^2 \geq n$." is a False premise.

C. The statement "If $n^2 \geq n$ and $n^2 \leq n$, then $n = n^2$." is a False premise.

D. All premises are true and therefore the argument is invalid.

E. Since 1 is not the largest positive integer, this argument cannot be valid.

---

**4.** (4 points) Using logical equivalences (NOT truth tables), prove that $\neg(p \rightarrow q) \rightarrow (\neg q)$ is a tautology. You may ONLY use the identities from Table 6, the first two from Table 7, and the first from Table 8. Do NOT skip or combine any steps.







---

**5.** (3 points) Determine the truth value of the following expression assuming that $p = T$, $q = F$, $r = T$, $s = F$.

$$[(p \leftrightarrow q) \rightarrow r] \oplus [(\neg r \land s) \rightarrow q]$$







---

**6.** For each positive integer $n$, let $A_n = \left[1 - \frac{1}{n}, ; 2^n\right)$. Determine the following sets:

(a) (2 points) $\displaystyle\bigcup_{n=1}^{\infty} A_n$





(b) (2 points) $\displaystyle\bigcap_{n=1}^{\infty} A_n$





---

**7.** Define the **diagonal** of two sets $A$ and $B$, denoted $A \triangle B$, to be the subset of $A \times B$ of ordered pairs with the first and second components equal. Written in set-builder notation:

$$A \triangle B = {(x, y) \in A \times B \mid x = y}.$$

(a) (1 point) For the sets $A = {1, 2, 3}$ and $B = {2, 3, 4}$, determine $A \triangle B$.



(b) (1 point) Give an example of nonempty sets $A$ and $B$ for which $A \triangle B = \varnothing$.




(c) (3 points) Prove or Disprove: If $A \triangle B = \varnothing$, then $A \cap B = \varnothing$.





---

**8.** (3 points) Prove that if $n$ is a positive integer, then $n$ is even if and only if $3n + 8$ is even.







---

**9.** (3 points) Prove that for any sets $A$ and $B$, if $\mathcal{P}(A) \subseteq \mathcal{P}(B)$, then $A \subseteq B$.











---

**10.** (3 points) Show that the argument form below is valid using a Step/Reason table listing the Rules of Inference and Logical Equivalences you use.

1. $p \rightarrow q$
2. $p \lor r$
3. $\neg r$
4. $\neg t \rightarrow \neg q$
5. $t \rightarrow (s \land u)$

$\therefore  u$