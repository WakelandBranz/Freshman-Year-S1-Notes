### Random Variables
 - A random variable is a numeric description of an experiment
	 - A discrete random variable may assume a finite number of values
	 - A continuous random variable may assume any numerical value in an interval.

---

### Discrete Probability Distribution
- The probability distribution for a random variable describes how probabilities are distributed over the values of the random variable.
- We can describe a discrete probability distribution with a table, graph, or formula.

---

### Binomial Distribution

Many problems in probability concern the repetition of an experiment having two possible outcomes. Each repetition of the experiment is called a **Bernoulli Trial**.

Suppose:
 - Each trial has **exactly two possible outcomes** referred to as a success and a failure. 
 - The trials are **independent**.
 - The probability of a success, denoted by **p**, is the same for every trial.
 - Your experiment consists of **n** trials.
If the random variable **X** represents the number of successes out of n trials, we say that X has a **binomial distribution.**

Let X be the total number of successes in **n Bernoulli trials** and let **p** be the probability of a success on each trial. Then the probability distribution of the random variable X is given by

$P(X = k) = _{n}C_{k} \cdot p^k \cdot (1 - p)^{n - k}$

The random variable X is called a **binomial random variable** and is said to have the **binomial distribution** with parameters ***n*** and ***p***.

---

### Binomial Coefficient

How do you count the number of ways to get k successes out of n trials? Remember, it's all about counting!

$\binom{n}{k} = {}_n C_k = \frac{n!}{k!(n-k)!}$

$_nC_k$ is referred to as the combination function. You read it as "n choose k."

---

