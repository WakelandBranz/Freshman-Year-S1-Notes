# Probability Concepts

## Set Operations

- **Union (A ∪ B)**: P(A) + P(B) - P(A ∩ B)
- **Intersection (A ∩ B)**: Probability of both events
- **From union**: P(A ∩ B) = P(A) + P(B) - P(A ∪ B)

## Conditional Probability

- **Formula**: P(A|B) = P(A ∩ B) / P(B)
- Given B occurred, what's probability of A?

## Independence vs Mutual Exclusivity

- **Independent**: P(A|B) = P(A) or P(A ∩ B) = P(A) × P(B)
- **Mutually Exclusive**: P(A ∩ B) = 0 (cannot both occur)
- If P(A ∩ B) ≠ 0, events are NOT mutually exclusive
- If P(A|B) ≠ P(A), events are NOT independent

---

# Hypothesis Testing

## P-values

- **If p-value < significance level (α)**: Reject null hypothesis
- **Smaller p-value**: More confident null hypothesis is false
- Common significance levels: 0.05, 0.01

## Null and Alternative Hypotheses

- **H₀ (null)**: Status quo, no difference/effect (usually has =)
- **Hₐ (alternative)**: What you're testing for (≠, <, or >)
- Example: H₀: μ = 940, Hₐ: μ < 940

## Making Conclusions

- If p-value < α: Reject H₀, conclude Hₐ is supported
- If p-value ≥ α: Fail to reject H₀, insufficient evidence

---

# Sampling Methods

## Population vs Sample

- **Population**: ALL members of the group being studied
- **Sample**: Subset selected from population for the study

## Sampling Types

- **Simple Random Sampling**: Each member has equal chance
- **Volunteer Sampling**: Self-selected participants
- **Convenience Sampling**: Easy-to-reach participants
- **Judgmental Sampling**: Expert selects participants

---

# CRISP-DM Phases

1. **Business Understanding**: Define objectives
2. **Data Understanding**: Explore and assess data quality
3. **Data Preparation**: Clean and transform data
4. **Modeling**: Build predictive models
5. **Evaluation**: Assess model performance
6. **Deployment**: Implement in production

---

# Machine Learning Types

## Supervised Learning

- **Classification**: Predict categorical outcomes (fraud/not fraud)
- **Regression**: Predict continuous numerical outcomes (price)

## Other Types

- **Unsupervised Learning**: Find patterns without labels (clustering)
- **Reinforcement Learning**: Learn through rewards/penalties

---

# Confusion Matrix Metrics

## Matrix Layout

|Prediction/Actual|Actual Negative (0)|Actual Positive (1)|
|---|---|---|
|**Predicted Negative (0)**|TN|FN|
|**Predicted Positive (1)**|FP|TP|

## Formulas

- **Accuracy** = (TP + TN) / (TP + TN + FP + FN)
- **Precision** = TP / (TP + FP)
- **Recall** = TP / (TP + FN)

---

# Linear Regression

## R-squared (R²)

- Percentage of variability in Y explained by X
- Ranges from 0 to 1
- R² = 0.743 means 74.3% of variability explained

## Interpreting Output

- **Coefficient (slope)**: Change in Y for 1-unit increase in X
- **Intercept**: Value of Y when X = 0
- **P-value (P>|t|)**: Tests if coefficient is significantly different from 0
- **P-value < 0.05**: Predictor is statistically significant

## Making Predictions

- Formula: Y = Intercept + (Slope × X)
- Use coefficients from regression output

## Statements About Models

- Positive slope means positive relationship
- Statistical significance ≠ causation
- Correlation does not imply causation

---