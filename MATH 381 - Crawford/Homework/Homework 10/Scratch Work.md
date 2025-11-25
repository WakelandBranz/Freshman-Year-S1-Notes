
> For this homework, formal proofs are not required, except for 9 and 10. You should provide at least some explanation for your answers.

---

## Problem 1

How many different three letter initials with none of the letters repeating can people have?

$P(26, 3) = \frac{26!}{(26 - 3)!} = \frac{26!}{23!} = 26 \cdot 25 \cdot 24$

---

## Problem 2

How many bit strings of length $n > 1$ begin and end with a 1?



---

## Problem 3

For $n > 1$, how many functions are there from the set ${1, \ldots, n}$ to the set ${0, 1}$?



---

## Problem 4

How many ways are there to seat 4 people from a group of 10 people around a circular table where two seatings are considered the same when everyone has the same neighbor, without regard to whether they are left or right neighbors.

$C(10, 4) = \frac{10!}{4!(10 - 4)!} = \frac{10!}{4!(6!)}$


---

## Problem 5

Let $S$ be the set of integers that are not divisible by 17 and let $T$ be any subset of $S$ so that $|T| = 308$. Show that there must be at least twenty integers in $T$ that have the same remainder when divided by 17.



---

## Problem 6

How many bit strings of length 12 contain:

**(a)** exactly three 1s

$6 \cdot 2^5$

**(b)** at most three 1s



**(c)** at least three 1s

**(d)** an equal number of 0s and 1s

---

## Problem 7

How many strings of six letters from the English alphabet contain:

**(a)** the letter a

**(b)** the letters a and b

**(c)** the letters a and b in consecutive positions with a preceding b and all the letters distinct

---

## Problem 8

What is the coefficient of $x^7$ in $(1 + x)^{11}$?

What are the coefficients of $x^6 y^9$ and $y^{14}$ in $(5x^2 + 2y^3)^6$?

---

## Problem 9 _(Formal Proof Required)_

Show that if $n$ is a positive integer then:

$$\binom{2n}{2} = 2\binom{n}{2} + n^2$$

---

## Problem 10 _(Formal Proof Required)_

Prove that for $n, r > 0$:

$$\sum_{k=0}^{r} \binom{n+k}{k} = \binom{n+r+1}{r}$$

**-PF-**