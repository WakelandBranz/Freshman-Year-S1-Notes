### Negation

- Little hook to notate a negation
- `"not¬ p"`

### Conjunction

- Little arrow pointing up to notate a conjunction
- You must have two propositions to make a conjunction
- `"p and∧ q"`

### Disjunction

- Little arrow pointing down to notate a disjunction
- `"p or q"`
- At least one must be true for the statement to evaluate to true
- If neither is true then the statement evaluates to false

### XOR (exclusive or)

- An **x** with a little circle around it to notate XOR
- `"p xor q"`
- **T** if _p_ is **T** & _q_ is **F**
- **T** if _p_ is **F** & _q_ is **T**
    - (essentially if one is true and the other is false then the statement evaluates to true… otherwise if they are both false or both true then the statement evaluates to false)
- **F** otherwise
    - Ex. _I will either use all of my savings to go to Jamaica, or I will buy a new car_

### Conditional Statement

- `p → q`
- `"p implies q"` **OR** `"If p, then q"`
- Is false if _q_ is false, but _p_ is true
- True otherwise
- [Lil Explanation](obsidian://open?vault=Obsidian%20Vault&file=MATH%20381%20-%20Crawford%2FSide%20notes%2FSection%201.1ish%20Side%20Notes)

### Biconditional

- `p ↔ q`
- Both _p_ implies _q_ and _q_ implies _p_
- `"p if and only if q"`
- `"q if and only if p"`
- Essentially both sides of the statement need to be the same for a true evaluation
- `"You can fly if you bought a plane ticket"`

### The **Converse**

- The converse of `p → q` is `q → p`
    - Base statement: _“I go running when it is sunny.”_
    - Converse: _“If it is sunny I go running.”_

### The **Inverse**

- The inverse of `p → q` is `not¬ p → not¬ q`
    - Base statement: _“I go running when it is sunny.”_
    - Inverse: _“If it is not sunny I do not go running.”_

### The **Contrapositive**

- The contrapositive of `p → q` is `not¬ q → not¬ p`
    - Base statement: _“I go running when it is sunny.”_
    - Contrapositive: _“If I am running it is not sunny.”_
### Truth Tables
- A row for each possible combination of Truth values for all of the propositions in your proposition
> [Useful truth table drawing](obsidian://open?vault=Obsidian%20Vault&file=MATH%20381%20-%20Crawford%2FTruth%20Table%20Example)

##### Example
- p = students who have taken 231 can take 232
- q = students who have taken comp 110 can take 381
- Conjunction - Students who have taken both 231 can take 232 and students who have taken 110 can take 381
- Disjunction - Students who have taken either 231 can take 232 or students who have taken comp 110 can take 381
- 