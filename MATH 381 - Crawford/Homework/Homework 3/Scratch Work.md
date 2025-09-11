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
If P(5) were to evaluate as true this does not imply that P(6), P(7), P(8), etc. would also evaluate as true.

---
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

### 2. Translate each of the following statements into logical expressions, introducing notation as needed for propositional functions and appropriate domains. Then negate the logical expression and translate the negation back into English.

##### (a) Some of the students in this class are not here today.

(Some people are both students and absent/not here)

S(x) = "x is a student in this class"
H(x) = "x is here today."

**Translation**: $\exists x(S(x) \land \lnot H(x))$
**Negation**: $\forall x(S(x) \rightarrow H(x))$

**English Negation**: All of the students in this class are here today. 

**Negation work**: 
1. $\lnot(\exists x(S(x) \land \lnot H(x)))$
2. $\equiv \forall x(\lnot (S(x) \land \lnot H(x)))$ - Negation of existential quantifier of 1.
3. $\equiv \forall x (\lnot S(x) \lor \lnot  (\lnot H(x)))$ - DeMorgan's Law of 2.
4. $\equiv \forall x(\lnot S(x) \lor H(x))$ - Double negation of 3.
5. $\equiv \forall x(S(x) \rightarrow H(x))$ - Logical equivalence of 4.

---
##### (b) The number $\sqrt{x}$ is rational if x is an integer

I(x) = "x is an integer"
R($\sqrt{x}$) = "$\sqrt{x}$ is rational"

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
1. $\lnot(\exists x (\forall y T(x, y) \land \forall z \forall y(T(z, y)) \rightarrow z = x)$
2. $\equiv \forall x(\lnot(\forall y T(x, y) \land \forall z \forall y(T(z, y)) \rightarrow z = x)))$ - Negation of the existential quantifier of 1.
3. $\equiv \forall x(\exists y(\lnot(T(x, y) \land \forall z \forall y(T(z, y)) \rightarrow z = x)))$ - Negation of the universal quantifier of 2.
4. $\equiv \forall x(\exists y(\lnot T(x, y))\lor \lnot(\forall z \forall y(T(z, y)) \rightarrow z = x))$ - DeMorgan's Law of 3.
5. $\equiv \forall x(\exists y(\lnot T(x, y)) \lor \exists z(\lnot(\forall y(T(x, y)) \rightarrow z = x)))$ - Negation of the universal quantifier of 4.
6. $\equiv \forall x(\exists y(\lnot T(x, y)) \lor \exists z \exists y(\lnot(T(x, y)) \rightarrow z = x))$ - Negation of the universal quantifier of 5.
7. $\equiv \forall x(\exists y(\lnot T(x, y)) \lor \exists z \exists y(\lnot (\lnot T(x, y)) \lor z = x))$ - Logical equivalence of 6.
8. $\equiv \forall x(\exists y(\lnot T(x, y)) \lor \exists z \exists y(T(x, y) (\lnot (\lor z = x))))$ - Double negation of 7.
9. $\equiv \forall x(\exists y(\lnot T(x, y)) \lor \exists z \exists y(T(x, y) \land \lnot z = x))$ - DeMorgan's Law of 8.

**Negation Work Try #2**: 
1. $\lnot (\exists x(\forall yT(x, y) \land \forall z (\forall yT(z, y)) \rightarrow z = x))$
2. $\equiv \lnot (\exists x(\forall yT(x, y) \land \forall z (\lnot(\forall yT(z, y))) \lor z = x))$ - Logical equivalence to 1.
3. $\equiv \forall x(\lnot (\forall yT(x, y) \land \forall z(\lnot(\forall yT(z, y))) \lor z = x))$ - Negation of the existential quantifier of 2.
4. $\equiv \forall x(\exists y(\lnot(T(x, y) \land \forall z(\lnot (\forall yT(z, y))) \lor z = x)))$ - Negation of the universal quantifier of 3.
5. $\equiv \forall x(\exists y \lnot T(x, y) \lor \lnot(\forall z(\lnot(\forall yT(z, y))) \lor z = x))$ - DeMorgan's Law of 4.
6. $\equiv \forall x(\exists y \lnot T(x, y) \lor \exists z(\lnot(\lnot(\forall yT(z, y))) \lor z = x))$ - Negation of the existential quantifier of 5.
7. $\equiv \forall x(\exists y \lnot T(x, y) \lor \exists z(\forall yT(z, y))\lnot (\lor z = x))$ - Double negation of 6.

**Negation Work Try #3**:
1. $\lnot(\exists x(\forall yT(x, y) \land \forall z(\forall yT(z, y) \rightarrow z = x)))$
2. $\equiv \forall x \lnot (\forall yT(x, y) \land \forall z(\forall yT(z, y) \rightarrow z = x))$ - Negation of the existential quantifier of 1.
3. $\equiv \forall x(\lnot (\forall yT(x, y)) \lor \lnot (\forall z(\forall yT(z, y) \rightarrow z = x)))$ - DeMorgan's Law of 2.
4. $\equiv \forall x(\exists y\lnot T(x, y) \lor \lnot(\forall z(\forall yT(z, y) \rightarrow z = x)))$ - Negation of the universal quantifier of 3.
5. $\equiv \forall x(\exists y\lnot T(x, y) \lor \exists z\lnot(\forall yT(z, y) \rightarrow z = x))$ - Negation of the universal quantifier of 4.
6. $\equiv \forall x(\exists y\lnot T(x, y) \lor \exists z(\lnot(\lnot(\forall yT(z, y)) \lor (z = x))))$ - Logical equivalence of 5. 
7. $\equiv \forall x(\exists y\lnot T(x, y) \lor \exists z(\lnot (\lnot (\forall yT(z, y))) \land \lnot (z = x)))$ - DeMorgan's Law of 6.
8. $\equiv \forall x(\exists y\lnot T(x, y) \lor \exists z(\forall yT(z, y) \land \lnot(z = x)))$ - Double negation of 7.
9. $\equiv \forall x(\exists y \lnot T(x, y) \lor \exists z(\forall yT(z, y)  \land z \neq x))$ - Negation of equality relation of 8.

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
##### (c) $\exists x \forall yP(x,y)$ 
This statement is false.
This statement states that there exists a value of x where all values of y result in P(x, y) evaluating to true. 
This is false, as for any fixed x, the equation x + 2y = xy can only be satisfied by at most one value of y.
Thus, since there is no x that works for all y, this statement is false.

---
### 5. Let the universe for m and for n be the set of positive integers an   d let the universe for z be the set of all integers. Write the negation of the following statement without the symbol “¬” and determine, with explanation, whether the original statement or its negation is true.

#### $\forall z \exists n \forall m (n \le z^2 \lor z < n + m)$

Can you show that z is true for all positive integers, all negative integers, and for zero, and then for n and m the positive integer.

For all values of z there exists a value of n that for all values of m such that $(n \le z^2 \lor z < n + m)$ is true.

**Negation**: $\exists z \forall n \exists m(n > z^2 \land z \ge n + m)$

**Negation Work:**
$\forall z \exists n \forall m (n \le z^2 \lor z < n + m)$
1. $\lnot (\forall z \exists n \forall m (n \le z^2 \lor z < n + m))$
2. $\equiv \exists z(\lnot (\exists n \forall m (n \le z^2 \lor z < n + m)))$ - Negation of the universal quantifier of 1.
3. $\equiv \exists z \forall n (\lnot (\forall m (n \le z^2 \lor z < n + m))))$ - Negation of the existential quantifier of 2.
4. $\equiv \exists z \forall n \exists m(\lnot(n \le z^2 \lor z < n + m))$ - Negation of the universal quantifier of 3.
5. $\equiv \exists z \forall n \exists m(n > z^2 \land z \ge n + m)$ - Negation of Inequality Relations of 2.

The original statement, $\forall z \exists n \forall m (n \le z^2 \lor z < n + m)$ is true. 
#### ***PF:***
For this proof, $n=1$. 
##### ***Case 1: z = 0***
- First disjunct: $(1 \leq 0)$
	- **False**
- Second disjunct: $(0 < 1 + m)$
	- Since $m \geq 1$, this statement must be true $(0 < 1 + 1..\infty)$
##### **Case 2: z $\neq$ 0**
 - First disjunct: $(1 \leq z^2)$
	 - For any non-zero integer z, $z^2 \geq 1$, therefore this disjunct is always true.
- Since the first disjunct is always true, the entire statement always evaluates to true therefore the second disjunct does not need to be evaluated.

Therefore, the original statement is true.

---
### 6. Let the universe for x be people and let the universe for y be movies. Translate the following statements to English without using any variables, given the following notation for predicates:

#### S(x, y): x saw y
#### L(x, y): x liked y
#### A(y): y won an award
#### C(y): y is a comedy

##### (a) $\forall y(C(y) \rightarrow \exists xL(x, y))$ 

***Rough Translation:*** For every movie, if it is a comedy movie then someone liked it.
##### Translation: Every comedy movie is liked by someone

---
##### (b) $\forall y \exists x(S(x, y) \land A(y))$

***Rough Translation:*** For every movie there exists someone who saw it and the movie won an award.
##### Translation: Every movie was seen by someone and won an award 