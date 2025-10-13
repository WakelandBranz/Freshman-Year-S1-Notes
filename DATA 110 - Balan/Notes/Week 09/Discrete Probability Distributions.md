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

### Python Math

```Python
from scipy.stats import binom

# Parameters
n = 10  # number of trials
p = 0.5  # probability of success
k = 3    # number of successes

# Probability Mass Function (PMF) - P(X = k)
pmf_value = binom.pmf(k, n, p)
print(f"P(X = {k}) = {pmf_value}")

# Cumulative Distribution Function (CDF) - P(X ≤ k)
cdf_value = binom.cdf(k, n, p)
print(f"P(X ≤ {k}) = {cdf_value}")
```

##### Common Use Cases

```Python
from scipy.stats import binom

n = 20   # flip 20 coins
p = 0.5  # fair coin

# Probability of exactly 10 heads
print(binom.pmf(10, n, p))

# Probability of 10 or fewer heads
print(binom.cdf(10, n, p))

# Probability of more than 10 heads: P(X > 10) = 1 - P(X ≤ 10)
print(1 - binom.cdf(10, n, p))

# Probability of at least 10 heads: P(X ≥ 10) = 1 - P(X ≤ 9)
print(1 - binom.cdf(9, n, p))

# Calculate for multiple values at once
k_values = [5, 10, 15]
pmf_values = binom.pmf(k_values, n, p)
print(pmf_values)
```

## Parameters

- **k**: number of successes (can be a single value or array)
- **n**: number of trials
- **p**: probability of success on each trial

### Other Useful Functions

```Python
# Survival function: P(X > k) = 1 - P(X ≤ k)
binom.sf(k, n, p)

# Mean and variance
mean = binom.mean(n, p)      # or simply n * p
variance = binom.var(n, p)   # or n * p * (1-p)

# Generate random samples
samples = binom.rvs(n, p, size=1000)
```

The key difference: **PMF** gives you the probability of an exact value, while **CDF** gives you the cumulative probability up to and including that value.

---
### Jobs Example

A student majoring in data science is trying to decide on the number of companies to which she should apply for a job. Given her work experience and grades, she expects that the probability of receiving a job offer from any individual company is 75%. Suppose that the student decides to apply to 6 companies.

1. 