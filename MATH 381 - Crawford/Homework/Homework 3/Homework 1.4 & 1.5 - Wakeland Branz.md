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
If P(5) were to evaluate as true this does not imply that P(6), P(7), P(8), etc. would also evaluate as true.

---
<div style="page-break-after: always;"></div>
page break above me


##### (c) $\forall x (2x \ge x)$, where the domain is $\mathbb{R}$.
This statement is false.
This statement attempts to claim that 2x is always greater than or equal to x for all real numbers but this is false for all negative numbers.
If $x \ge 0$ then this statement evaluates to true, but it is false otherwise. 
If x were to equal -1, then the statement would evaluate to $(2(-1) \ge -1) \equiv (-2 \ge -1)$ which is false.
 
---
##### (d) $\exists x (x^2 = e^x)$, where the domain is $\mathbb{R}$.

This statement is true.
$e^x$ and $x^2$ are both continuous functions for all real numbers.
The difference of continuous functions is continuous.
Therefore, $f(x) = e^x - x^2$ is continuous for $\mathbb{R}$.
$f(x) = e^x - x^2$
$f(0) = e^0 - 0^2 = 1 - 0 = 1$
$f(-1) = e^{-1} - (-1)^2 = 1/e - 1 \approx 0.368 - 1 = -0.632 < 0$
$f(x)$ is continuous on the interval [-1, 0].
$f(-1) < 0$ and $f(0) > 0$ thus 0 lies between $f(-1)$ and $f(0)$.
By the intermediate value theorem, there exists some value z such that $f(z) = 0$.
$f(z) = 0$ means $e^z - z^2 = 0$
Therefore $e^z = z^2$ proves $\exists x(x^2 = e^x)$ is true.

---
<div style="page-break-after: always;"></div>
page break above me

### 2. Translate each of the following statements into logical expressions, introducing notation as needed for propositional functions and appropriate domains. Then negate the logical expression and translate the negation back into English.

##### (a) Some of the students in this class are not here today.

S(x) = "x is a student in this class"
H(x) = "x is here today."

**Translation**: $\exists x(S(x) \land \lnot H(x))$
**Negation**: $\forall x(S(x) \rightarrow H(x))$

**English Negation**: All of the students in this class are here today. 

**Negation work**: 
1. $\lnot(\exists x(S(x) \land \lnot H(x)))$
2. $\equiv \forall x(\lnot (S(x) \land \lnot H(x)))$ - Existential quantifier to universal quantifier of 1.
3. $\equiv \forall x (\lnot S(x) \lor \lnot  (\lnot H(x)))$ - DeMorgan's Law of 2.
4. $\equiv \forall x(\lnot S(x) \lor H(x))$ - Double negation of 3.
5. $\equiv \forall x(S(x) \rightarrow H(x))$ - Logical equivalence of 4.

---
##### (b) The number $\sqrt{x}$ is rational if x is an integer

I(x) = "x is an integer"
R($\sqrt{x}$) "$\sqrt{x}$ is rational"

**Translation**: $\forall x(I(x) \rightarrow R(\sqrt{x}))$
**Negation**: $\exists x(I(x) \land \lnot R(\sqrt{x}))$
**English Negation**: There exists an integer x such that $\sqrt{x}$ is irrational.

**Negation Work**: 
1. $\lnot(\forall x(I(x) \rightarrow R(\sqrt{x})))$
2. $\equiv \lnot(\forall x(\lnot I(x) \lor R(\sqrt{x})))$ - Logical Equivalence to 1.
3. $\equiv \exists x(\lnot  (\lnot I(x) \lor R(\sqrt{x})))$ - Negation of universal quantifier of 2.
4. $\equiv \exists x(\lnot (\lnot I(x)) \land \lnot R(\sqrt{x}))$ - DeMorgan's Law of 3.
5. $\exists x(I(x) \land \lnot R(\sqrt{x}))$ - Double negation of 4.
---
### 3. Let the domain for x be teachers at UNC and the domain for y be classes at UNC. Translate the following English statements into logical expressions, using the below:

#### T(x, y): $x$ is teaching $y$
#### M(y): $y$ is a math course

#### x: Teachers at UNC
#### y: Classes at UNC

#### Then give the negation of your logical expression, simplifying as much as possible.

##### (a) Every teacher at UNC teaches at least one math course.

**Translation**: $\forall x \exists y(T(x, y) \land M(y))$
**Negation**: $\exists x \forall y(\lnot T(x, y) \lor \lnot M(y))$

**Negation Work**: 
1. $\lnot(\forall x \exists y(T(x, y) \land M(y)))$
2. $\equiv \exists x(\lnot(\exists y(T(x, y) \land M(y))))$ - Negation of the universal quantifier of 1.
3. $\equiv \exists x \forall y(\lnot(T(x, y) \land M(y)))$ - Negation of the existential quantifier of 2.
4. $\equiv \exists x \forall y(\lnot T(x, y) \lor \lnot M(y))$ - DeMorgan's Law of 2.

---
##### (b) There is exactly one teacher who teaches every class at UNC
#### x: Teachers at UNC
#### y: Classes at UNC

#### Let z have the domain of teachers at UNC

**Translation**: $\exists x (\forall y T(x, y) \land \forall z( \forall yT(z, y) \rightarrow z = x))$
**Negation**: $\forall x(\exists y \lnot T(x, y) \lor \exists z(\forall yT(z, y)  \land z \neq x))$

 - $\exists x \forall yT(x, y)$
	 - This part represents "There exists at least one teacher who teaches every class at UNC"
- $\forall z \forall y(T(z,y)) \rightarrow z = x$
	- This part represents exactly one teacher

**Negation Work**:
1. $\lnot(\exists x(\forall yT(x, y) \land \forall z(\forall yT(z, y) \rightarrow z = x)))$
2. $\equiv \forall x \lnot (\forall yT(x, y) \land \forall z(\forall yT(z, y) \rightarrow z = x))$ - Negation of the existential quantifier of 1.
3. $\equiv \forall x(\lnot (\forall yT(x, y)) \lor \lnot (\forall z(\forall yT(z, y) \rightarrow z = x)))$ - DeMorgan's Law of 2.
4. $\equiv \forall x(\exists y\lnot T(x, y) \lor \lnot(\forall z(\forall yT(z, y) \rightarrow z = x)))$ - Negation of the universal quantifier of 3.
5. $\equiv \forall x(\exists y\lnot T(x, y) \lor \exists z\lnot(\forall yT(z, y) \rightarrow z = x))$ - Negation of the universal quantifier of 4.
6. $\equiv \forall x(\exists y\lnot T(x, y) \lor \exists z(\lnot(\lnot(\forall yT(z, y)) \lor (z = x))))$ - Logical equivalence of 5. 
7. $\equiv \forall x(\exists y\lnot T(x, y) \lor \exists z(\lnot (\lnot (\forall yT(z, y))) \land \lnot (z = x)))$ - DeMorgan's Law of 6.
8. $\equiv \forall x(\exists y\lnot T(x, y) \lor \exists z(\forall yT(z, y) \land \lnot(z = x)))$ - Double negation of 7.
9. $\equiv \forall x(\exists y \lnot T(x, y) \lor \exists z(\forall yT(z, y)  \land z \neq x))$ - Negation of equality relation of 8.

