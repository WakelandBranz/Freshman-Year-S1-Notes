### Statistical Experiments
> A random experiment is any process that yields an observation whose outcome cannot be known in advance.

An **outcome** is any particular result of an experiment.

An **event** is a subset of outcomes of an experiment
 - Simple event = single outcome
 - Complex event = a set of two or more simple events.

The **sample space** is the set of all possible outcomes of an experiment.
 
 ---

### Probability
- The **probability** of an event is a number that measures the relative likelihood that the event will occur.
- The probability assigned to each experimental outcome must be between 0 and 1, inclusively.
- The sum of the probabilities for all experimental outcomes must equal 1.

---

### Assigning Probabilities

 - **Classical Method**: Assigns probabilities based on the assumption of equally likely outcomes (dice, for example).
 - **Relative Frequency Method**: Assigns probabilities based on experimentation or historical data.
	 - **Long-run frequency / law of large numbers**: As the number of trials increases, the empirical probability approaches the theoretical (true) probability.
- **Subjective Method**: Assigns probabilities based on judgement.

---

### **Some Basic Relationships of Probability**

 - The **complement** of event $A$ (denoted by $\overline A$ or $A^c$) consists of everything in the sample space that is NOT in $A$.
 - The **union** ($\cup$) of two events $A$ and $B$ consists of all of the outcomes that are in $A$ or $B$ or both.
 - The **intersection** ($\cap$) of two events $A$ and $B$ consists of all of the outcomes that are in **BOTH** $A$ and $B$.
 - Two events $A$ and $B$ are **mutually exclusive** if they have no outcomes in common (e.g., the intersection of $A$ and $B$ is empty). IN other words, the events $A$ and $B$ cannot occur simultaneously.

---

### Law of Addition

For any two events $A$ and $B$
 - $P ( A \cup B) = P(A) + P(B) - P(A \cap B)$

If two $A$ and $B$ are mutually exclusive, then
 - $P (A \cup B) = P(A) + P(B)$

---

### Conditional Probability

The probability of an event $A$ **given** that event $B$ has occurred is a **conditional probability** and is denoted by $P ( A \mid B)$ 

For any two events $A$ and $B$:
	$P(A \mid B) = \frac{P(A \cup B)}{P(B)}$
and
	$P (A \mid B) = \frac{P(A \cup B)}{P(A)}$

---

### Independence

If knowing that an event $B$ has occurred does **NOT** affect the probability that event $A$ will occur, then events $A$ and $B$ are **independent events**.

Equivalently, two events $A$ and $B$ are independent if and only if:

> $P (A \mid B) = P(A)$ or
> $P (B \mid A) = P(A)$

---

### Law of Multiplication

> For any two events $A$ and $B$

$P(A \cap B) = P(A \mid B) * P(B)$

> If events $A$ and $B$ are independent, then

$P(A \cap B) = P(A) * P(B)$

---

### Example

Apple products have become a household name in America with 51% of all households  
owning at least one Apple product (CNN, March 19, 2012). The probability of owning  
an Apple product is 61% for households with kids and 48% for households without  
kids. Suppose that 68% of households have kids and the rest are without kids.  

 - What is the probability that a household selected at random has kids and owns at  least one Apple product?  
	 - $P( 1A \cap K) = P(1A \mid K) * P(K) = \frac{P(1A \cup K)}{P(K)} * P(K) = 0.41$
 - What is the probability that a household selected at random does not own an Apple  product?  
 - Are having kids and owning an Apple product mutually exclusive events? Why or  why not?  
 - Are having kids and owning an Apple product independent events? Why or why not?