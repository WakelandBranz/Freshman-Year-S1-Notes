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

(Some people are both students and absent)

S(x) = "x is a student in this class"
H(x) = "x is here today."

**Translation**: $\exists x(S(x) \land \lnot H(x))$
**Negation**: $\forall x(S(x) \rightarrow H(x))$

**English Negation**: All of the students in this class are here today. 

**Negation work**: 
$\lnot(\exists x(S(x) \land \lnot H(x)))$
1. $\equiv \lnot \exists x (\lnot (S(x)) \land \lnot H(x)))$ - Distributing out the negation
2. $\equiv \forall x (\lnot S(x) \lor \lnot  (\lnot H(x)))$ - DeMorgan's Law
3. $\equiv \forall x(\lnot S(x) \lor H(x))$ - Double negation
$\equiv \forall x(S(x) \rightarrow H(x))$ - Logical equivalence

---
##### (b) The number $\sqrt{x}$ is rational if x is an integer

I(x) = "x is an integer"
R($\sqrt{x}$) "$\sqrt{x}$ is rational"

**Translation**: $\forall x(I(x) \rightarrow R(\sqrt{x}))$
**Negation**: $\exists x(I(x) \land \lnot R(\sqrt{x}))$

**English Negation**: There exists an integer x such that $\sqrt{x}$ is irrational.

**Negation Work**: 
1. $\forall x(I(x) \rightarrow R(\sqrt{x}))$
2. $\equiv \forall x(\lnot I(x) \lor R(\sqrt{x}))$ - Logical Equivalence to 1.
3. $\lnot (\forall x(\lnot I(x) \lor R(\sqrt{x})))$ - Begin distribution of the negative
4. $\equiv \lnot \forall x(\lnot (\lnot I(x) \lor R(\sqrt{x})))$ - Distribution of the negative
5. $\equiv \lnot \forall x(\lnot (\lnot I(x)) \lnot \lor \lnot R(\sqrt{x}))$  - Distribution of the negative
6. $\equiv \exists x(\lnot(\lnot I(x) \land \lnot R(\sqrt{x})))$ - DeMorgan's Law of 5.
7. $\equiv \exists x(I(x) \land \lnot R(\sqrt{x}))$ - Double Negation of 6.

---

### 3. Let the domain for x be teachers at UNC and the domain for y be classes at UNC. Translate the following English statements into logical expressions, using the below:

#### T(x, y): $x$ is teaching $y$
#### M(y): $y$ is a math course

#### Then give the negation of your logical expression, simplifying as much as possible.

##### (a) Every teacher at UNC teaches at least one math course.

---
##### (b) There is exactly one teacher who teaches every class at UNC

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
When simplified, $2 + 2y = 2y \equiv 2 = 0$, thus when x = 2 there does not exist a value of y such that P(x, y) evaluates to true.
This means that the entire statement is false.

---
##### (c) $\exists x \forall yP(x,y)$ ===REVIEW THIS===
This statement is false.
This statement states that there exists a value of x where all values of y result in P(x, y) evaluating to true. 
This is false, as for any fixed x, the equation x + 2y = xy can only be satisfied by at most one value of y.
Thus, since there is no x that works for all y, this statement is false.

---

### 5. Let the universe for m and for n be the set of positive integers and let the universe for z be the set of all integers. Write the negation of the following statement without the symbol “¬” and determine, with explanation, whether the original statement or its negation is true.

#### $\forall z \exists n \forall m (n \le z^2 \lor z < n + m)$

For all values of z there exists a value of n that for all values of m $(n \le z^2 \lor z < n + m)$ is true.

**Negation**: 

**Negation Work:**
1. $\forall z \exists n \forall m (n \le z^2 \lor z < n + m)$


---
### 6. Let the universe for x be people and let the universe for y be movies. Translate the following statements to English without using any variables, given the following notation for predicates:

#### S(x, y): x saw y
#### L(x, y): x liked y
#### A(y): y won an award
#### C(y): y is a comedy

##### (a) $\forall y(C(y) \rightarrow \exists xL(x, y))$ 

---
##### (b) $\forall y \exists x(S(x, y) \land A(y))$