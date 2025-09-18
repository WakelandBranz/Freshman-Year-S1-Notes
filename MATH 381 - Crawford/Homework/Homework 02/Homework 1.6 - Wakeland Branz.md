### 1.
#### A)
Determine if the following argument forms are valid or invalid. Explain your reasoning.

$\begin{align} p &\implies q \\ p &\implies r \\ \hline \therefore q &\implies r \end{align}$
##### Counterexample
- p = "Sarah gets an A on the final exam"
- q = "Sarah is happy"
- r = "Sarah calls her parents"
$p \rightarrow q$ - If Sarah gets an A on the final exam, then she is happy.
$p \rightarrow r$ - If Sarah gets an A on the final exam, then Sarah calls her parents.
$\therefore q \rightarrow r$ - Therefore, if Sarah is happy, then Sarah calls her parents.

This logic is not valid. 
While Sarah being happy as a result of getting an A on her final exam and Sarah calling her parents as a result of getting an A on the final exam do make sense, there is a litany of other possible reasons as to why Sarah could be calling her parents other than her being happy. 
The premises only tell us what happens when Sarah aces the final, but the conclusion incorrectly assumes that ALL of Sarah's happiness leads to calling her parents. 
This shows the logical gap in the argument structure.

---
<br> <br> <br> <br> <br> <br> <br> <br> <br>
#### B)
$\begin{align} (p \rightarrow q) &\land (r \rightarrow s) \\ p &\lor r \\ \hline \therefore q &\lor s\end{align}$

#### PF:  
1. $(p \rightarrow q) \land (r \rightarrow s)$ - Premise
2. $(p \rightarrow q)$ - Simplification of 1 
3.  $p \lor r$ - Premise
4. $r \rightarrow s$ - Simplification of 1
5. $\lnot p \lor q$ - Logical Equivalence of 2
6. $\lnot r \lor s$ - Logical Equivalence of 4
7. $q \lor r$ - Resolution of 3 and 5
8. $r \lor p$ - Commutative law of 3
9. $p \lor s$ - Resolution of 6 and 8
10. $r \lor q$ - Commutative of 7
11. $q \lor s$ - Resolution of 10 and 6

Based on the proof above, this argument form is valid.

---
 <br> <br> <br> <br> <br> <br> <br>

 <br> <br> <br> <br> <br> <br>
 <br>
 <br>

#### C)
 $\begin{align} (\lnot p \lor \lnot q) &\rightarrow (r \land s) \\ r &\rightarrow t \\ \lnot t \\ \hline \therefore p\end{align}$

#### PF:  
1. $r \rightarrow t$ - Premise
2. $\lnot t$ - Premise
3. $\lnot r$ - Modus Tollens on 1 & 2
4. $\lnot r \lor \lnot s$ - Addition of 3
5. $\lnot (r \land s)$ - DeMorgan's Law on 4
6. $(\lnot p \lor \lnot q) \rightarrow (r \land s)$ - Premise
7. $\lnot(\lnot p \lor \lnot q)$ - Modus Tollens on 5 and 6
8. $\lnot (\lnot p) \land \lnot(\lnot q)$ - DeMorgan's Law on 7
9. $p \land q$ - Double Negation
10. $p$ - Simplification

Based on the proof above, this argument form is valid.

---
 <br> <br> <br> <br> <br> <br>

 <br> <br> <br> <br> <br> <br>
 <br> <br> <br>
### 2. 

Suppose that the argument from with premises $p_{1}$, $...$, $p_n$, $q$ and conclusion $r$ is valid. Show that this implies that the argument form with premises $p_{1}$, $...$, $p_{n}$ and conclusion $q \rightarrow r$.

$\begin{align} &p_{1} \\ &\dots \\ &p_{n} \\ &q \\ \hline &r \end{align}$

$\begin{align} &p_{1} \\ &\dots \\ &p_{n} \\ \hline &q \rightarrow r \end{align}$

Given that the first argument is valid, we know whenever all premises, $p_{1}$, ..., $p_{n}$, $q$ are true, then $r$ must be true.
For our second argument to be valid, we need to show that whenever $p_{1}$, ..., $p_{n}$ are all true, then $q \rightarrow r$ must be true.
For the second argument o fail, $q \rightarrow r$ would have to be false, which only happens when $q$ is true and $r$ is false.
In any cases where $p_{1}$, ..., $p_{n}$ are all true.
If $q$ is false, then $q \rightarrow r$ is automatically true.
If $q$ is true, then we have $p_{1}$, ..., $p_{n}$, $q$ all true.
Since the original argument was valid, this forces $r$ to be true, making $q \rightarrow r$ true as well.
Therefore $q \rightarrow r$ is true in both cases, so the second argument is valid.

---
 <br> <br> <br> <br> <br> <br> <br> <br> <br> <br>
 <br>
 <br>
### 3. 

Use exercise (**2**) to show that the argument form with premises $(p \land t) \rightarrow (r \lor s)$, $q \rightarrow (u \land t)$, $u \rightarrow p$, and $\lnot s$ and conclusion $q \rightarrow r$ is valid.

Given premises:

$\begin{align}  (p \land t) &\rightarrow (r \lor s) \\ q &\rightarrow (u \land t) \\ u &\rightarrow p \\ &\lnot s \\ \hline \therefore q &\rightarrow r\end{align}$

$\equiv$

$\begin{align}  (p \land t) &\rightarrow (r \lor s) \\ q &\rightarrow (u \land t) \\ u &\rightarrow p \\ &\lnot s \\ &q \\ \hline &r\end{align}$

Based on what we proved in exercise 2, the above 2 argument forms are equivalent. 
To use exercise 2's method, we assume $q$ is true and show that $r$ must follow.
From $q$ being true and the premise $q \rightarrow (u \land t)$, we can conclude $(u \land t)$ is true using modus ponens.
From $(u \land t)$ being true, we can extract that both $u$ and $t$ are individually true.
Since $u$ is true and we have the premise $u \rightarrow p$, we can conclude $p$ is true using modus ponens.
Now we know both $p$ and $t$ are true, so $(p \land t)$ is true.
From $(p \land t)$ being true and the premise $(p \land t) \rightarrow (r \lor s)$, we can conclude $(r \lor s)$ is true using modus ponens.
We also have the premise $\lnot s$ (s is false).
Since $(r \lor s)$ is true and $s$ is false, $r$ must be true using disjunctive syllogism.
Therefore, assuming $q$ leads us to conclude $r$.
By using exercise 2, this proves that $q \rightarrow r$ is a valid conclusion from our original premises.

---
 <br> <br> <br>
  <br>
### 4. 

Below is a "proof" that $-\frac{1}{2}$ is positive. Is this a valid argument? 
If so, explain why we were able to deduce a false conclusion from a valid argument. 
If not, explain.

"We know that if $0 \leq x^2 \leq 1$, then $0 \leq x \leq 1$ for any real number x.
Clearly $(-\frac{1}{2})^2 = 1/4$ is between 0 and 1.
Therefore $-\frac{1}{2}$ is between 0 and 1."

This argument uses correct logical reasoning (modus ponens), making it valid. 
Despite this, the first premise is **false.**

The premise claims "if $0 \leq x^2 \leq 1$, then $0 \leq x \leq 1$" but this is incorrect.
The correct premise would be "if $0 \leq x^2 \leq 1$, then $-1 \leq x \leq 1$" since both positive and negative values can have squares in this range.
We were able to deduce a false conclusion from a valid argument in this scenario because valid arguments with false premises can produce false conclusions.
Since $-\frac{1}{2}$ satisfies $0 \leq x^2 \leq 1$ but does not satisfy the (incorrect) conclusion $0 \leq x \leq 1$, we see the premise is false.
The logical structure is correct, but the false premise leads to a false conclusion.

---
<br> <br> <br>
  <br>
  <br> <br> <br>
  <br>
  <br><br><br>
### 5.

Show that the following is a valid argument: 

"Becky either works in a hospital or at a tech startup. If they work at a hospital, Becky must have seen several injuries. But Becky as not seen any injuries. It must be that Becky works at a tech startup."

p = Works in a hospital
q = Works in a tech startup
r = Seen several injuries

$\begin{align} p &\lor q \\ p &\rightarrow r \\ &\lnot r \\ \hline &\therefore q\end{align}$

#### PF:  
1. $p \lor q$ - Premise
2. $p \rightarrow r$ - Premise
3. $\lnot r$ - Premise
4. $\lnot p$ -  Modus Tollens of 2 and 3
5. $q$ - Disjunctive Syllogism of 1 and 4

Based on the proof above, this is a valid argument.

---
### 6.
Find ONE example of the following (you do not need to find all three) on social media, a podcast, the news, or other source:
(a) An example of a valid argument which as true premises and a true conclusion.
===(b) An example of a valid argument which includes at least one false premise.===
(c) An example of an invalid argument, meaning that it has true premises leading to a false conclusion.
####  Pew Research article showing an example of a valid argument which includes at least one false premise
- https://www.pewresearch.org/science/2023/08/09/why-some-americans-do-not-see-urgency-on-climate-change/
- _“I believe it’s cyclical. And the reason why I believe this is because there were record high temperatures more than 100 years ago that are higher than what we are having now. And this is going to come and go as time goes on – a.k.a. cyclical.”_ –Woman, 50s, Coastal Florida
#### PF:
- P = "Past temperatures (100+ years ago) were higher than current temperatures"
- Q = "Current warming is part of natural cycles"
- R = "Current warming is natural/not human-caused"

1. $p$ - Premise (false)
2. $p \rightarrow q$ - Premise (questionable)
3. $q \rightarrow r$ - Premise (questionable)
4. $q$ - Modus Ponens of 1 and 2
5. $r$ - Modus Ponens of 3 and 4

This example demonstrates a valid argument with a false premise because while the logical reasoning follows correctly (if past temperatures were higher, then warming is cyclical, therefore current warming is natural), the factual claim that past temperatures exceeded current ones is scientifically incorrect, making the argument structurally sound but factually flawed.

---