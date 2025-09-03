### 1.
#### A)

$\begin{align} p &\implies q \\ p &\implies r \\ \hline \therefore q &\implies r \end{align}$
##### Counterexample
- p = "Sarah gets an A on the final exam"
- q = "Sarah is happy"
- r = "Sarah calls her parents"
$p \rightarrow q$ - If Sarah gets an A on the final exam, then she is happy.
$p \rightarrow r$ - If Sarah gets an A on the final exam, then Sarah calls her parents.
$\therefore q \rightarrow r$ - Therefore, if Sarah is happy, then Sarah calls her parents.

This logic is not valid. While Sarah being happy as a result of getting an A on her final exam and Sarah calling her parents as a result of getting an A on the final exam do make sense, there is a litany of other possible reasons as to why Sarah could be calling her parents other than her being happy. The premises only tell us what happens when Sarah aces the final, but the conclusion incorrectly assumes that ALL of Sarah's happiness leads to calling her parents. This shows the logical gap in the argument structure.



















#### B)
$\begin{align} (p \rightarrow q) &\land (r \rightarrow s) \\ p &\lor r \\ \hline \therefore q &\lor s\end{align}$

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

This argument form is valid.

#### C)
 $\begin{align} (\lnot p \lor \lnot q) &\rightarrow (r \land s) \\ r &\rightarrow t \\ \lnot t \\ \hline \therefore p\end{align}$

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

This argument form is valid.
