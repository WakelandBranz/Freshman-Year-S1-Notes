**NOTE:** To receive partial credit please show your work in detail OR write down the form of the Python function that you used to compute the probability (e.g., `binom.pmf(3, 15, 0.1)`).

---

## Problem 1

A company maintains a pool of loaner laptops for special projects. Each laptop has a 10% probability of not working. You are putting together a small team to work on a new project, and you select 14 laptops for the team to use.

### 1a. (2 points)

What is the probability that exactly half of them won't work?

```Python
binom.pmf(7, 14, 0.1)
```

$\binom{14}{7} \left( \frac{1}{10} \right)^7 * \left( \frac{9}{10} \right)^7 = 0.00016415149608$ 

### 1b. (2 points)

What is the probability that all of them will work?

```Python
binom.pmf(0, 14, 0.1)
```

$\binom{14}{0} \left( \frac{9}{10} \right)^{14} = 0.2287679245496099$

### 1c. (2 points)

What is the probability that fewer than 3 of them will not work?

```Python
binom.cdf(2, 14, 0.1)
```

$0.84164001871338$

---

## Problem 2 (3 points)

You are planning to purchase a toy robot for your nephew's birthday. The robot has 5 electronic components. There is a 1% probability that any one of the components will be defective. If two or more of the components are defective, the robot will not function properly. What is the probability that the toy robot you purchase for your nephew will not function properly when he takes it out of the box?

```Python
1 - binom.cdf(2, 5, 0.01)
```
$\binom{5}{2}$

---

## Problem 3

A survey of a magazine's subscribers indicates that 50% of the subscribers own a house, 80% own a car, and 90% of the homeowners also own a car.

### 3a. (2 points)

What is the probability that a randomly selected subscriber owns both a car and a house?

### 3b. (2 points)

What is the probability that a randomly selected subscriber does not own a house?

### 3c. (2 points)

What is the probability that a randomly selected subscriber owns either a house or a car?

---

## Problem 4 (3 points)

In a four-cylinder engine, there are four spark plugs. If any one of them malfunctions, the car will idle roughly and power will be lost. Suppose that for a certain brand of spark plugs, the probability that a spark plug will function properly after 5000 miles is 0.9. Assuming that the spark plugs operate independently, what is the probability that the car will idle roughly after 5000 miles?

---

## Problem 5

The Department of Parks and Recreation recently conducted a survey designed to gain a better understanding of how residents were utilizing greenways. The survey indicated that 33% of residents jog while 42% of the residents bike. However, 29% of the bikers also jog.

### 5a. (2 points)

What is the probability that a resident selected at random utilizes the greenway for both biking and jogging?

### 5b. (2 points)

Are biking and jogging mutually exclusive events?

### 5c. (2 points)

Are biking and jogging independent events?

---

## Problem 6

There is a 14% chance that a Noodles and Company customer will order bread with their meal. Suppose that we take a random sample of 10 customers.

### 6a. (2 points)

What is the probability that more than 5 will order bread?

### 6b. (2 points)

What is the probability that no more than 2 will order bread?

### 6c. (2 points)

What is the probability that none of the 10 will order bread?

---