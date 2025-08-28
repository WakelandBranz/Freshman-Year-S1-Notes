
| Rule of inference (premises ⊢ conclusion) | Tautology (always true) | Name |
|---|---|---|
| $p \rightarrow q,\; p \;\vdash\; q$ | $((p \rightarrow q)\land p)\rightarrow q$ | Modus Ponens |
| $p \rightarrow q,\; \lnot q \;\vdash\; \lnot p$ | $((p \rightarrow q)\land \lnot q)\rightarrow \lnot p$ | Modus Tollens |
| $p \rightarrow q,\; q \rightarrow r \;\vdash\; p \rightarrow r$ | $((p \rightarrow q)\land (q \rightarrow r))\rightarrow (p \rightarrow r)$ | Hypothetical Syllogism |
| $p \lor q,\; \lnot p \;\vdash\; q$ | $((p \lor q)\land \lnot p)\rightarrow q$ | Disjunctive Syllogism |
| $p \;\vdash\; p \lor q$ | $p \rightarrow (p \lor q)$ | Addition (Disjunction Introduction) |
| $p \land q \;\vdash\; p$ | $((p \land q)\rightarrow p)$ | Simplification (∧‑Elimination ₁) |
| $p \land q \;\vdash\; q$ | $((p \land q)\rightarrow q)$ | Simplification (∧‑Elimination ₂) |
| $p,\; q \;\vdash\; p \land q$ | $((p)\land (q))\rightarrow (p \land q)$ | Conjunction (∧‑Introduction) |
| $p \lor q,\; \lnot p \lor r \;\vdash\; q \lor r$ | $((p \lor q)\land (\lnot p \lor r))\rightarrow (q \lor r)$ | Resolution |
- **Turnstile (⊢)** = “we can **prove** this."
- **Therefore (∴)** = “as a result, **hence**."