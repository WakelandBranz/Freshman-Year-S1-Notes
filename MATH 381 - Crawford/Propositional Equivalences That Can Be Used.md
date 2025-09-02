## THE ONLY THINGS WE CAN USE FOR LOGICAL EQUIVALENCES IS TABLE 6, TABLE 7 ROWS 1 & 2, TABLE 8 ROW 1 IN THE BOOK AND WHAT IS BELOW

##### DeMorgan's Laws
- ¬(p ∧ q) ≡ ¬p ∨ ¬q
- ¬(p ∨ q) ≡ ¬p ∧ ¬q

- p ⊕ q ≡ (p ∨ q) ∧ ¬(p ∧ q)
- p ⊕ q ≡ q ⊕ p
- p ∧ T ≡ p

# Logical Equivalences Tables

## Table 6: Logical Equivalences

|Equivalence|Name|
|---|---|
|p ∧ T ≡ p|Identity laws|
|p ∨ F ≡ p||
|p ∨ T ≡ T|Domination laws|
|p ∧ F ≡ F||
|p ∨ p ≡ p|Idempotent laws|
|p ∧ p ≡ p||
|¬(¬p) ≡ p|Double negation law|
|p ∨ q ≡ q ∨ p|Commutative laws|
|p ∧ q ≡ q ∧ p||
|(p ∨ q) ∨ r ≡ p ∨ (q ∨ r)|Associative laws|
|(p ∧ q) ∧ r ≡ p ∧ (q ∧ r)||
|p ∨ (q ∧ r) ≡ (p ∨ q) ∧ (p ∨ r)|Distributive laws|
|p ∧ (q ∨ r) ≡ (p ∧ q) ∨ (p ∧ r)||
|¬(p ∧ q) ≡ ¬p ∨ ¬q|De Morgan's laws|
|¬(p ∨ q) ≡ ¬p ∧ ¬q||
|p ∨ (p ∧ q) ≡ p|Absorption laws|
|p ∧ (p ∨ q) ≡ p||
|p ∨ ¬p ≡ T|Negation laws|
|p ∧ ¬p ≡ F||

## Table 7: Logical Equivalences Involving Conditional Statements

| Equivalence                     |
| ------------------------------- |
| ==p → q ≡ ¬p ∨ q==              |
| ==p → q ≡ ¬q → ¬p==             |
| p ∨ q ≡ ¬p → q                  |
| p ∧ q ≡ ¬(p → ¬q)               |
| ¬(p → q) ≡ p ∧ ¬q               |
| (p → q) ∧ (p → r) ≡ p → (q ∧ r) |
| (p → r) ∧ (q → r) ≡ (p ∨ q) → r |
| (p → q) ∨ (p → r) ≡ p → (q ∨ r) |
| (p → r) ∨ (q → r) ≡ (p ∧ q) → r |

## Table 8: Logical Equivalences Involving Biconditional Statements

| Equivalence                     |
| ------------------------------- |
| ===p ↔ q ≡ (p → q) ∧ (q → p)=== |
| p ↔ q ≡ ¬p ↔ ¬q                 |
| p ↔ q ≡ (p ∧ q) ∨ (¬p ∧ ¬q)     |
| ¬(p ↔ q) ≡ p ↔ ¬q               |
