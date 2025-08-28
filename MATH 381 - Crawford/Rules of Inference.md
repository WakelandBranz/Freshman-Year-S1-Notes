
| Rule of inference (premises ⊢ conclusion)                       | Tautology (always true)                                                   | Name                                |
| --------------------------------------------------------------- | ------------------------------------------------------------------------- | ----------------------------------- |
| $p \rightarrow q,\; p \;\vdash\; q$                             | $((p \rightarrow q)\land p)\rightarrow q$                                 | Modus Ponens                        |
| $p \rightarrow q,\; \lnot q \;\vdash\; \lnot p$                 | $((p \rightarrow q)\land \lnot q)\rightarrow \lnot p$                     | Modus Tollens                       |
| $p \rightarrow q,\; q \rightarrow r \;\vdash\; p \rightarrow r$ | $((p \rightarrow q)\land (q \rightarrow r))\rightarrow (p \rightarrow r)$ | Hypothetical Syllogism              |
| $p \lor q,\; \lnot p \;\vdash\; q$                              | $((p \lor q)\land \lnot p)\rightarrow q$                                  | Disjunctive Syllogism               |
| $p \;\vdash\; p \lor q$                                         | $p \rightarrow (p \lor q)$                                                | Addition (Disjunction Introduction) |
| $p \land q \;\vdash\; p$                                        | $((p \land q)\rightarrow p)$                                              | Simplification (∧‑Elimination ₁)    |
| $p \land q \;\vdash\; q$                                        | $((p \land q)\rightarrow q)$                                              | Simplification (∧‑Elimination ₂)    |
| $p,\; q \;\vdash\; p \land q$                                   | $((p)\land (q))\rightarrow (p \land q)$                                   | Conjunction (∧‑Introduction)        |
| $p \lor q,\; \lnot p \lor r \;\vdash\; q \lor r$                | $((p \lor q)\land (\lnot p \lor r))\rightarrow (q \lor r)$                | Resolution                          |
- **Turnstile (⊢)** = “we can **prove** this."
- **Therefore (∴)** = “as a result, **hence**."
Sure! Below is the same information, but each rule is laid out **vertically** (one block per rule).  
You can copy‑paste this markdown directly into Obsidian or any other markdown editor.

---
# Vertical Version

### Modus Ponens  
**Inference (premises ⊢ conclusion)**  
`p → q ,  p ⊢ q`  

**Tautology (always true)**  
`((p → q) ∧ p) → q`  

**Name**  
Modus Ponens  

---  

### Modus Tollens  
**Inference**  
`p → q ,  ¬q ⊢ ¬p`  

**Tautology**  
`((p → q) ∧ ¬q) → ¬p`  

**Name**  
Modus Tollens  

---  

### Hypothetical Syllogism  
**Inference**  
`p → q ,  q → r ⊢ p → r`  

**Tautology**  
`((p → q) ∧ (q → r)) → (p → r)`  

**Name**  
Hypothetical Syllogism  

---  

### Disjunctive Syllogism  
**Inference**  
`p ∨ q ,  ¬p ⊢ q`  

**Tautology**  
`((p ∨ q) ∧ ¬p) → q`  

**Name**  
Disjunctive Syllogism  

---  

### Addition (Disjunction Introduction)  
**Inference**  
`p ⊢ p ∨ q`  

**Tautology**  
`p → (p ∨ q)`  

**Name**  
Addition  

---  

### Simplification (∧‑Elimination ₁)  
**Inference**  
`p ∧ q ⊢ p`  

**Tautology**  
`(p ∧ q) → p`  

**Name**  
Simplification (∧‑E₁)  

---  

### Simplification (∧‑Elimination ₂)  
**Inference**  
`p ∧ q ⊢ q`  

**Tautology**  
`(p ∧ q) → q`  

**Name**  
Simplification (∧‑E₂)  

---  

### Conjunction (∧‑Introduction)  
**Inference**  
`p , q ⊢ p ∧ q`  

**Tautology**  
`(p ∧ q) ← (p ∧ q)`  *(or equivalently `(p ∧ q) → (p ∧ q)`) – a trivial truth*  

**Name**  
Conjunction  

---  

### Resolution  
**Inference**  
`p ∨ q ,  ¬p ∨ r ⊢ q ∨ r`  

**Tautology**  
`((p ∨ q) ∧ (¬p ∨ r)) → (q ∨ r)`  

**Name**  
Resolution  

---  

*Feel free to adjust the wording or formatting (e.g., use blockquotes, definition lists, or a single‑column table) to match your preferred style.*