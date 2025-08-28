Here’s the same three‑column table, but the **first column** now shows each inference **vertically** (premise 1, premise 2, …, turnstile, conclusion).

| Rule of inference (vertical)     | Tautology (always true)               | Name                                |
| -------------------------------- | ------------------------------------- | ----------------------------------- |
| `p → q`<br>`p`<br>`⊢ q`          | `((p → q) ∧ p) → q`                   | Modus Ponens                        |
| `p → q`<br>`¬q`<br>`⊢ ¬p`        | `((p → q) ∧ ¬q) → ¬p`                 | Modus Tollens                       |
| `p → q`<br>`q → r`<br>`⊢ p → r`  | `((p → q) ∧ (q → r)) → (p → r)`       | Hypothetical Syllogism              |
| `p ∨ q`<br>`¬p`<br>`⊢ q`         | `((p ∨ q) ∧ ¬p) → q`                  | Disjunctive Syllogism               |
| `p`<br>`⊢ p ∨ q`                 | `p → (p ∨ q)`                         | Addition (Disjunction Introduction) |
| `p ∧ q`<br>`⊢ p`                 | `(p ∧ q) → p`                         | Simplification (∧‑E₁)               |
| `p ∧ q`<br>`⊢ q`                 | `(p ∧ q) → q`                         | Simplification (∧‑E₂)               |
| `p`<br>`q`<br>`⊢ p ∧ q`          | `(p ∧ q) → (p ∧ q)` *(trivial truth)* | Conjunction (∧‑Introduction)        |
| `p ∨ q`<br>`¬p ∨ r`<br>`⊢ q ∨ r` | `((p ∨ q) ∧ (¬p ∨ r)) → (q ∨ r)`      | Resolution                          |

*Each premise (or set of premises) is listed on its own line, followed by the turnstile **⊢** and the conclusion, giving a clear vertical layout of the argument.*

- **Turnstile (⊢)** = “we can **prove** this."
- **Therefore (∴)** = “as a result, **hence**."
