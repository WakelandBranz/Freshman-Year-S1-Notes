
> For this homework, formal proofs are not required, except for 9 and 10. You should provide at least some explanation for your answers.

---

## Problem 1

How many different three letter initials with none of the letters repeating can people have?

$P(26, 3) = \frac{26!}{(26 - 3)!} = \frac{26!}{23!} = 26 \cdot 25 \cdot 24$

---

## Problem 2

How many bit strings of length $n > 1$ begin and end with a 1?

$2^{n - 2}$

---

## Problem 3

For $n > 1$, how many functions are there from the set ${1, \ldots, n}$ to the set ${0, 1}$?

I viewed this as binary strings
$2^n$

---

## Problem 4

How many ways are there to seat 4 people from a group of 10 people around a circular table where two seatings are considered the same when everyone has the same neighbor, without regard to whether they are left or right neighbors.


How many ways are there to seat 4 people from a group of 10 people around a circular table where two seatings are considered the same when everyone has the same neighbor, without regard to whether they are left or right neighbors.

$C(10, 4) = \frac{10!}{4!(10 - 4)!} = \frac{10!}{4!(6!)}$

With regard to whether they are left or right neighbors, any set of 4 people from the group of 10 people has $\frac{4!}{4}$ seating arrangements.
Without regard to whether they are left or right neighbors, this is halved, so $\frac{4!}{4} / 2$.

**Final answer:** $[\frac{10!}{4!(10-4)!} \cdot \frac{4!}{4}] / 2$

---

## Problem 5

Let $S$ be the set of integers that are not divisible by 17 and let $T$ be any subset of $S$ so that $|T| = 308$. Show that there must be at least twenty integers in $T$ that have the same remainder when divided by 17.

Since there are 16 integers in the domain of $\pmod{17}$, there are 308 integers ("objects") and 16 potential remainders ("boxes") so we must find $\lceil \frac{308}{16} \rceil$.

$\lceil \frac{|T|}{16} \rceil = \lceil \frac{308}{16} \rceil = \lceil 19.25 \rceil = 20$.

---

## Problem 6

How many bit strings of length 12 contain:

**(a)** exactly three 1s

$\frac{12!}{3!(12 - 3)!}$

**(b)** at most three 1s

$1 + (\frac{12!}{1!(12 - 1)!}) + (\frac{12!}{2!(12 - 2)!}) + (\frac{12!}{3!(12 - 3)!})$

**(c)** at least three 1s

$2^{12} - [1 + (\frac{12!}{1!(12 - 1)!}) + (\frac{12!}{2!(12 - 2)!}]$

**(d)** an equal number of 0s and 1s

$\frac{12!}{6!(12 - 6)!}$

---

## Problem 7

How many strings of six letters from the English alphabet contain:

**(a)** the letter a

$26^6 - 25^6$

**(b)** the letters a and b

$26^6 - 2 \cdot 25^6 + 24^6$

**(c)** the letters a and b in consecutive positions with a preceding b and all the letters distinct

$(24 \cdot 23 \cdot 22 \cdot 21) \cdot 5$

---

## Problem 8

What is the coefficient of $x^7$ in $(1 + x)^{11}$?]

$\binom{11}{7} = \frac{11!}{7!(11 - 7)!} = \frac{11!}{(7!)(4!)}$

What are the coefficients of $x^6 y^9$ and $y^{14}$ in $(5x^2 + 2y^3)^6$?

$a = 5x^2, b = 2y^3, n = 6$
$\sum_{k = 0}^6 \binom{6}{k}(5x^2)^{6 - k}(2y^3)^k$
 For $k = 3: \binom{6}{3} \cdot 5^3 \cdot 2^3$
 Coefficient of $x^6y^9 = \binom{6}{3} \cdot 5^3 \cdot 2^3$

Coefficient of $y^{14} = 0$ because there is no $k$ such that $x$'s exponent is 0 and $y$'s exponent is $14$.

---

## Problem 9 _(Formal Proof Required)_

Show that if $n$ is a positive integer then:

$$\binom{2n}{2} = 2\binom{n}{2} + n^2$$

**-PF-**
Show that if $n$ is a positive integer then:

$$\binom{2n}{2} = 2\binom{n}{2} + n^2$$

First, we must simplify the left side of the equality.
$\binom{2n}{2} = \frac{(2n)!}{(2!)(2n - 2)!}$
$\frac{1}{(2n - 2)!} = \frac{(2n)(2n-1)}{(2n)!}$
So, $\frac{(2n)!}{(2!)(2n - 2)!} = \frac{(2n)!(2n)(2n - 1)}{(2!)(2n)!} = \frac{(2n)(2n - 1)}{(2!)} =  \frac{(2n)(2n - 1)}{(2)} = \frac{4n^2 - 2n}{2} = 2n^2 - n$
Second, we must simplify the right side of the equality.
$2 \binom{n}{2} + n^2 = 2(\frac{n!}{(2!)(n - 2)!}) + n^2 = 2(\frac{n!}{(2)(n - 2)!}) + n^2 = \frac{n!}{(n - 2)!} + n^2$
$\frac{1}{(n - 2)!}  = \frac{(n)(n - 1)}{n!}$
So, $\frac{n!}{(n - 2)!} + n^2 = \frac{(n!)(n)(n - 1)}{n!} + n^2 = (n)(n-1) + n^2 = n^2 - n + n^2 = 2n^2 - n$
We have now proven that both $\binom{2n}{2} = 2n^2 - n$ and $2\binom{n}{2} + n^2 = 2n^2 - n$.
Thus $\binom{2n}{2} = 2\binom{n}{2} + n^2$ is true.

---

## Problem 10 _(Formal Proof Required)_

Prove that for $n, r > 0$:

$$\sum_{k=0}^{r} \binom{n+k}{k} = \binom{n+r+1}{r}$$

**-PF-**