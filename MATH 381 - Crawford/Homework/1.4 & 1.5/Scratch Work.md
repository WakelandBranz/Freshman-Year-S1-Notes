---

---
---
### 1. Determine if the following propositions are True or False. Provide an explanation for each one.

##### (a) $\forall x P(x) \rightarrow \exists P(x)$, where P(x) is an arbitrary propositional function.
This statement is **true** (and a tautology).
In order for this statement to evaluate to false, the first proposition must be true and the second must be false. 
This is not possible in this case though--if the first proposition evaluates to true, the second must also evaluate to true.
Since the first proposition being true implies that P(x) evaluates to true for all values of x, then there must exist an x for which P(x) will evaluate to true for the second proposition (all values of x will).

---
##### (b) $\exists x P(x) \rightarrow \forall x P(x)$ is an arbitrary propositional function

This statement is false.
This statement attempts to claim that if some values of x are true for P(x) then all values of x are true for P(x).
This cannot be true.
If P(x) were to be $x = 5$ then the first proposition would evaluate as true because there exists a case where $x = 5$ thus P(5) is true but P(6) is false so $\forall xP(x)$ is false.

---
##### (c) $\forall x (2x \ge x)$, where the domain is $\mathbb{R}$.

This statement is false.
This statement attempts to claim that 2x is always greater than or equal to x for all real numbers but this is false for all negative numbers.
If $x \ge 0$ then this statement evaluates to true, but it is false otherwise. 
If x were to equal -1, then the statement would evaluate to $(2(-1) \ge -1) \equiv (-2 \ge -1)$ which is false.
 
---
##### (d) $\exists x (x^2 = e^x)$, where the domain is $\mathbb{R}$.
 
---

### 2. Translate each of the following statements into logical expressions, introducing notation as needed for propositional functions and appropriate domains. Then negate the logical expression and translate the negation back into English.

##### (a) Some of the students in this class are not here today.

S(x) = "x is a student in this class"
H(x) = "x is here today."

Translation: $\exists x(S(x) \land \lnot H(x))$
Negation: 

##### (b)

---

### 3. 

---
### 4. Let P (x, y) be the statement x + 2y = xy, where x is an integer and y is a real number. Determine the truth value of each statement, with explanation.
##### (a) $\exists yP(4,y)$
This statement is true.
P(4, y) can be evaluated as $4 + 2y = 4y$. 
Algebraically, this statement is equivalent to $4 = 2y$ which tells us that when y = 2 this statement is true.
Since this statement asks if there exists a value where it evaluates to true, and since P(4, y) evaluates to true when y = 2, this statement is true.

---
##### (b) $\forall x \exists yP(x,y)$
This statement is false.
When x = 2, P(2, y) evaluates to $2 + 2y = 2y$. 
$2 + 2y = 2y$ is a false statement, thus when x = 2 there does not exist a value of y such that P(x, y) evaluates to true.
This means that the entire statement is false.

---
##### (c) $\exists x \forall yP(x,y)$

---
