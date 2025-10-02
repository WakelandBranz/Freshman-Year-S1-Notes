## 1. Propositional Logic

### Proposition
A declarative statement that is either true or false, but not both.

**Examples:**
- "It is raining" (can be T or F)
- "2 + 2 = 4" (T)
- "Is it sunny?" (NOT a proposition - it's a question)

### Negation (¬p)
The opposite truth value of a proposition.

**Example:** If p = "It is sunny", then ¬p = "It is not sunny"

### Conjunction (p ∧ q)
True only when both propositions are true; "and" operator.

**Example:** p = "I have a ticket", q = "The show is tonight"
- p ∧ q = "I have a ticket AND the show is tonight"

### Disjunction (p ∨ q)
True when at least one proposition is true; "or" operator.

**Example:** p = "It rains", q = "It snows"
- p ∨ q = "It rains OR it snows" (true if either or both occur)

### Exclusive Or (p ⊕ q)
True when exactly one proposition is true, but not both.

**Example:** "I will either go to Jamaica or buy a car" (but not both)

### Conditional Statement (p → q)
"If p, then q" - false only when p is true and q is false.

**Example:** "If it rains (p), then I bring an umbrella (q)"
- False only when it rains but I don't bring an umbrella

### Biconditional (p ↔ q)
"p if and only if q" - true when both have the same truth value.

**Example:** "You can fly if and only if you have a ticket"
- True when both happen or both don't happen

### Converse
The converse of p → q is q → p.

**Example:** 
- Original: "If it's sunny, I run"
- Converse: "If I run, it's sunny"

### Inverse
The inverse of p → q is ¬p → ¬q.

**Example:**
- Original: "If it's sunny, I run"
- Inverse: "If it's not sunny, I don't run"

### Contrapositive
The contrapositive of p → q is ¬q → ¬p.

**Example:**
- Original: "If it's sunny, I run"
- Contrapositive: "If I'm not running, it's not sunny"

### Tautology
A compound proposition that is always true regardless of truth values.

**Example:** p ∨ ¬p ("It's sunny or it's not sunny" - always true)

### Contradiction
A compound proposition that is always false.

**Example:** p ∧ ¬p ("It's sunny and it's not sunny" - always false)

### Contingency
A proposition whose truth value depends on its component propositions.

**Example:** p ∨ q (truth depends on values of p and q)

### Logical Equivalence (p ≡ q)
Two propositions are logically equivalent when p ↔ q is a tautology.


**Example:** p → q ≡ ¬p ∨ q

## 2. Predicates and Quantifiers

### Subject
The variable or thing in a statement.

**Example:** In "x > 3", x is the subject

### Predicate
The property that the subject possesses.

**Example:** In "x > 3", "> 3" (greater than 3) is the predicate

### Propositional Function
A statement containing variables that becomes a proposition when values are assigned.

**Example:** P(x) = "x > 3" becomes a proposition when x = 5

### Domain
The collection of possible values for variables.

**Example:** For P(x) = "x is even", domain could be ℤ (all integers)

### Counterexample
A specific value that makes a universal statement false.

**Example:** For "∀x(x² > x)", x = 0 is a counterexample since 0² = 0

### Universal Quantification (∀xP(x))
"For all x, P(x) is true" - must be true for every element in the domain.

**Example:** ∀x(x + 1 > x) over ℝ means "every real number plus 1 is greater than itself"

### Existential Quantification (∃xP(x))
"There exists an x such that P(x)" - true if at least one element satisfies P(x).

**Example:** ∃x(x² = 4) over ℤ is true (x = 2 or x = -2)

### Nested Quantifiers
Quantifiers within the scope of other quantifiers.

**Example:** ∀x∃y(x + y = 0) means "for every x, there exists a y such that x + y = 0"

## 3. Arguments and Inference

### Argument
A sequence of propositions (premises) leading to a conclusion.

**Example:**
- Premise 1: If it's sunny, I play football
- Premise 2: It is sunny
- Conclusion: I play football

### Valid Argument
An argument where the truth of premises guarantees the truth of the conclusion.

**Example:** Modus Ponens is valid: (p → q) ∧ p ⊢ q

### Sound Argument
A valid argument with true premises.

**Example:** 
- "All humans are mortal" (true)
- "Socrates is human" (true)
- "Therefore, Socrates is mortal" (valid and sound)

### Modus Ponens
Inference rule: If p → q and p are true, then q is true.

**Example:** "If it rains, the ground is wet" + "It rains" → "The ground is wet"

## 4. Proof Techniques

### Theorem
An important statement that can be proven true.

**Example:** "If n is odd, then n² is odd"

### Proposition
A less important theorem.

**Example:** "The sum of two even numbers is even"

### Axiom (Postulate)
A statement assumed to be true without proof.

**Example:** "For any two points, there exists exactly one line through them"

### Proof
A valid logical argument showing a theorem is true.

### Lemma
A smaller proposition used to prove a larger theorem.

**Example:** Proving "√2 is irrational" might first prove "if n² is even, then n is even" as a lemma

### Corollary
A theorem that follows directly from another theorem.

**Example:** After proving "if n is odd, then n² is odd", the corollary "if n² is even, then n is even" follows

### Conjecture
A statement believed to be true but not yet proven.

**Example:** Goldbach's Conjecture: "Every even integer > 2 is the sum of two primes"

### Direct Proof
Assume p is true, then show q must be true to prove p → q.

**Example:** To prove "if n is odd, then n² is odd":
- Assume n = 2k + 1
- Then n² = 4k² + 4k + 1 = 2(2k² + 2k) + 1, which is odd

### Proof by Contraposition
Prove ¬q → ¬p instead of p → q.

**Example:** To prove "if 3n + 2 is odd, then n is odd":
- Prove instead: "if n is even, then 3n + 2 is even"
- If n = 2k, then 3n + 2 = 6k + 2 = 2(3k + 1), which is even

### Proof by Contradiction
Assume the negation of what you want to prove, derive a contradiction.

**Example:** To prove √2 is irrational:
- Assume √2 = a/b in lowest terms
- Derive that both a and b must be even
- Contradiction: they can't both be even if in lowest terms

### Proof by Cases
Split the domain into cases and prove each separately.

**Example:** Prove n² ≥ n for all integers:
- Case 1: n < 0 (negative squared is positive ≥ negative)
- Case 2: n = 0 (0² = 0)
- Case 3: n > 0 (n·n ≥ 1·n)

### Exhaustive Proof
Check all possible cases when the number is small.

**Example:** Prove (n+1)³ ≥ 3ⁿ for n ≤ 4:
- Check n = 1, 2, 3, 4 individually

### Without Loss of Generality (WLOG)
Reduce cases by recognizing symmetry.

**Example:** To prove |xy| = |x||y|, can assume x ≤ 0 WLOG since the case y ≤ 0 is symmetric

### Existence Proof (Constructive)
Explicitly find an element satisfying the property.

**Example:** "∃n that's a sum of two cubes two ways": 1729 = 10³ + 9³ = 12³ + 1³

### Existence Proof (Non-constructive)
Prove something exists without explicitly finding it.

**Example:** Prove ∃ irrational x, y with xʸ rational using √2^√2

### Uniqueness Proof
Show (1) something exists and (2) it's the only one.

**Example:** Prove ax + b = 0 has unique solution when a ≠ 0:
- Existence: x = -b/a works
- Uniqueness: if ax + b = 0 and as + b = 0, then ax = as, so x = s

## 5. Sets

### Set
An unordered collection of distinct objects called elements.

**Example:** A = {1, 2, 3}, B = {red, blue, green}

### Element (∈)
An object belonging to a set.

**Example:** 2 ∈ {1, 2, 3} but 4 ∉ {1, 2, 3}

### Roster Notation
Listing all elements in braces.

**Example:** {1, 2, 3, 4, 5}

### Set Builder Notation
{x | condition on x} reads "the set of all x such that condition holds".

**Example:** {x ∈ ℤ | x is odd} = {x | ∃k ∈ ℤ, x = 2k + 1}

### Empty Set (∅)
The set with no elements; also written {}.

**Example:** {x ∈ ℤ | 0 < x < 1} = ∅

### Singleton Set
A set with exactly one element.

**Example:** {0}, {∅}

### Set Equality
Sets A and B are equal if they have exactly the same elements.

**Example:** {1, 2, 3} = {3, 1, 2} = {1, 1, 2, 3}

### Universal Set (U)
The set containing all objects under consideration.

**Example:** When discussing integers, U = ℤ

### Subset (A ⊆ B)
Every element of A is also in B.

**Example:** {1, 2} ⊆ {1, 2, 3, 4}

### Superset (B ⊇ A)
B contains all elements of A.

**Example:** {1, 2, 3, 4} ⊇ {1, 2}

### Proper Subset (A ⊂ B)
A ⊆ B and A ≠ B.

**Example:** {1, 2} ⊂ {1, 2, 3}

### Finite Set
A set with a countable number of elements.

**Example:** {1, 2, 3, 4, 5} has |A| = 5

### Infinite Set
A set that is not finite.

**Example:** ℕ = {1, 2, 3, ...}, ℝ

### Cardinality (|A|)
The number of elements in a set.

**Example:** |{a, b, c}| = 3

### Power Set (𝒫(A))
The set of all subsets of A.

**Example:** 𝒫({1, 2}) = {∅, {1}, {2}, {1, 2}}
- If |A| = n, then |𝒫(A)| = 2ⁿ

### Ordered n-tuple
An ordered collection (a₁, a₂, ..., aₙ).

**Example:** (1, 2) ≠ (2, 1); coordinate pairs like (3, 4)

### Cartesian Product (A × B)
The set of all ordered pairs (a, b) where a ∈ A and b ∈ B.

**Example:** {1, 2} × {a, b} = {(1,a), (1,b), (2,a), (2,b)}
- |A × B| = |A| · |B|

### Relation
A subset of A × B.

**Example:** R = {(1, 2), (2, 3)} is a relation on {1, 2, 3}

## 6. Set Operations

### Union (A ∪ B)
Elements in A or B or both.

**Example:** {1, 2, 3} ∪ {3, 4, 5} = {1, 2, 3, 4, 5}

### Intersection (A ∩ B)
Elements in both A and B.

**Example:** {1, 2, 3} ∩ {2, 3, 4} = {2, 3}

### Disjoint Sets
Sets with no common elements; A ∩ B = ∅.

**Example:** {1, 2} and {3, 4} are disjoint

### Set Difference (A - B)
Elements in A but not in B.

**Example:** {1, 2, 3} - {2, 3, 4} = {1}

### Complement (Ā or Aᶜ)
All elements in the universal set U not in A.

**Example:** If U = {1, 2, 3, 4, 5} and A = {1, 2}, then Ā = {3, 4, 5}

### De Morgan's Laws (Sets)
- ‾‾‾‾‾‾‾(A ∪ B) = Ā ∩ B̄
- ‾‾‾‾‾‾‾(A ∩ B) = Ā ∪ B̄

**Example:** Not (red or blue) = (not red) and (not blue)

### Cardinality Formula
|A ∪ B| = |A| + |B| - |A ∩ B|

**Example:** A = {1, 2, 3}, B = {2, 3, 4}
- |A ∪ B| = 3 + 3 - 2 = 4

### Distributive Laws
- A ∩ (B ∪ C) = (A ∩ B) ∪ (A ∩ C)
- A ∪ (B ∩ C) = (A ∪ B) ∩ (A ∪ C)

## 7. Functions

### Function
A relation where each element in the domain maps to exactly one element in the codomain.

**Example:** f: ℤ → ℤ defined by f(x) = x²

### Domain
The set of all possible inputs for a function.

**Example:** For f(x) = x², domain = ℝ

### Codomain
The set where outputs are taken from.

**Example:** For f: ℤ → ℤ with f(x) = x², codomain = ℤ

### Range
The set of actual outputs produced by the function.

**Example:** For f: ℤ → ℤ with f(x) = x², range = {0, 1, 4, 9, 16, ...} (non-negative perfect squares)

### Preimage
The set of inputs that map to a given output.

**Example:** For f(x) = x², preimage of 4 is {-2, 2}

### Equal Functions
Functions f and g are equal if they have the same domain, codomain, and f(x) = g(x) for all x.

**Example:** f(x) = x² - 1 and g(x) = (x-1)(x+1) are equal functions

### Injective (One-to-One)
A function where different inputs produce different outputs; if f(x₁) = f(x₂), then x₁ = x₂.

**Example:** f(x) = x + 1 is injective (each output comes from one input)
**Non-example:** f(x) = x² is not injective (f(-2) = f(2) = 4)

### Surjective (Onto)
A function where every element in the codomain is mapped to by at least one element in the domain.

**Example:** f: ℤ → ℤ with f(x) = x + 1 is surjective (every integer is hit)
**Non-example:** f: ℤ → ℤ with f(x) = x² is not surjective (negative integers are never outputs)

### Bijective
A function that is both injective and surjective.

**Example:** f: ℝ → ℝ with f(x) = 2x + 3 is bijective

### Inverse Function (f⁻¹)
For a bijective function f: A → B, f⁻¹: B → A reverses the mapping.

**Example:** If f(x) = 2x + 3, then f⁻¹(x) = (x - 3)/2

### Composition (f ∘ g)
(f ∘ g)(x) = f(g(x)) - apply g first, then f.

**Example:** If f(x) = x² and g(x) = x + 1, then (f ∘ g)(x) = (x + 1)²

### Floor Function (⌊x⌋)
The greatest integer less than or equal to x.

**Example:** ⌊3.7⌋ = 3, ⌊-2.3⌋ = -3

### Ceiling Function (⌈x⌉)
The smallest integer greater than or equal to x.

**Example:** ⌈3.2⌉ = 4, ⌈-2.3⌉ = -2

## 8. Number Theory Definitions

### Even Integer
An integer n where n = 2k for some integer k.

**Example:** 4 = 2(2), -6 = 2(-3), 0 = 2(0)

### Odd Integer
An integer n where n = 2k + 1 for some integer k.

**Example:** 7 = 2(3) + 1, -3 = 2(-2) + 1

### Rational Number
A real number that can be expressed as a/b where a, b ∈ ℤ and b ≠ 0.

**Example:** 1/2, -3/4, 5 = 5/1

### Irrational Number
A real number that is not rational.

**Example:** √2, π, e

### Perfect Square
An integer n where n = k² for some integer k.

**Example:** 9 = 3², 16 = 4², 0 = 0²

## Common Set Notations

- **ℕ** = {1, 2, 3, ...} (natural numbers)
- **ℤ** = {..., -2, -1, 0, 1, 2, ...} (integers)
- **ℤ⁺** = {1, 2, 3, ...} (positive integers)
- **ℚ** = {a/b | a, b ∈ ℤ, b ≠ 0} (rational numbers)
- **ℝ** = real numbers
- **ℂ** = complex numbers

## Key Logical Equivalences

1. **De Morgan's Laws:**
   - ¬(p ∧ q) ≡ ¬p ∨ ¬q
   - ¬(p ∨ q) ≡ ¬p ∧ ¬q

2. **Conditional Equivalences:**
   - p → q ≡ ¬p ∨ q
   - p → q ≡ ¬q → ¬p (contrapositive)
   - ¬(p → q) ≡ p ∧ ¬q

3. **Quantifier Negations:**
   - ¬(∀xP(x)) ≡ ∃x(¬P(x))
   - ¬(∃xP(x)) ≡ ∀x(¬P(x))

## Proof Strategy Quick Reference

| Goal | Method |
|------|--------|
| Prove p → q directly | Assume p, derive q |
| Prove p → q when direct is hard | Prove contrapositive: ¬q → ¬p |
| Prove p (single statement) | Assume ¬p, derive contradiction |
| Prove p ↔ q | Prove p → q AND q → p |
| Prove ∃xP(x) | Find one example where P(x) is true |
| Prove ∀xP(x) | Take arbitrary x, show P(x) |
| Multiple cases to consider | Proof by cases (cover all cases) |
| Small finite set | Exhaustive proof (check all) |
| Show something is unique | Prove existence, then show uniqueness |

---

*Tags: #discrete-math #logic #sets #functions #proofs #quantifiers*