## Review: Real Estate Example

**Scenario:** You have been hired by a local real estate investor who is interested in understanding what factors influence home prices in his area. He will use this information to:

- Help set prices for homes he is preparing to sell
- Make decisions about which homes to buy
- Determine how to renovate homes he currently owns

**Dataset:** Homes sold between 2006 and 2010

---

## Interpreting the Slope

**Key Concept:** The slope is the change in $y$ for a 1-unit change in $x$ (holding everything else constant).

**Example Question:** Suppose you are thinking about renovating your garage to fit one additional car. The cost of the renovation is estimated to be $25,000. You only want to do the renovation if you could recoup the cost when you sell the house. Should you do the renovation?

**Solution:** The slope for `GarageCars` is $3.878 \times 10^4$ or $38,780. This means that you would expect a $38,780 increase in sales price if you increased the number of cars that can fit into the garage by 1.

Since the expected increase ($38,780) exceeds the renovation cost ($25,000), the renovation is worthwhile.

---

## Making a Prediction

**Example:** Suppose you are interested in purchasing a house with the following characteristics:

- 2-car garage
- 1,100 square feet on the first floor
- Lot area of 10,000 square feet
- 3 bedrooms on the main floor
- 2 full bathrooms

How much should you expect to pay?

**Calculation:** $$\text{SalePrice} = -27,910 + (38,780 \times 2) + (66.71 \times 1100) + (0.6246 \times 10,000) - (773.516 \times 3) + (37,310 \times 2)$$

$$= $201,577$$

---

## Assessing the Model: Variable Significance

In order to determine whether an explanatory variable is a useful predictor, you can conduct a hypothesis test to determine whether the slope of the line is equal to zero or not.

**Hypothesis Test:**

- $H_0: \beta_1 = 0$ (x does not have a significant influence on the response)
- $H_a: \beta_1 \neq 0$ (x does have a significant influence on the response)

**Rule of Thumb:** In practice, a good model should have all (or most) x-variables to be significant at the 5% significance level.

---

## Assessing the Model: R-squared

The **Coefficient of Determination** (better known as the R-squared value) tells you the percentage of variability in $Y$ that can be explained by the variables in the regression model.

**Properties:**

- $0 \leq R^2 \leq 1$
- You want to see $R^2$ values approaching 1
- In practice, anything greater than 0.5 would probably be considered a fairly good model

**Warning:** When analyzing real data, if you get $R^2 = 1$ (or very close to 1), it probably means that you have done something wrong!

---

## Categorical Variables in Regression

**Key Points:**

- Categorical variables can be used as explanatory variables in a regression model, but they must first be converted to numeric variables
- **Dummy (or indicator) variables** are used to represent categorical variables
- If a categorical variable has $c$ levels, then you will need $c-1$ indicator variables to represent it

---

## Example: Kitchen Quality

In our exploratory analysis of these data, we noticed that there seem to be some differences in the prices of homes based on the quality of the kitchen. Suppose that we want to include Kitchen Quality in our regression analysis.

**Kitchen Quality** is a categorical variable with four levels: `Ex`, `Fa`, `Gd`, `Ta`

`Ex` (Excellent) becomes the **base case** to which we compare all of the other levels.

**Dummy Variable Encoding:**

|KitchenQual|Kitchen_Fa|Kitchen_Gd|Kitchen_Ta|
|---|---|---|---|
|Ex|0|0|0|
|Fa|1|0|0|
|Gd|0|1|0|
|Ta|0|0|1|

---

## Linear Regression in Python

Linear regression can be implemented in Python using libraries such as:

- `scikit-learn`
- `statsmodels`

**Common output includes:**

- Coefficients (`coef`)
- Standard errors (`std err`)
- t-statistics (`t`)
- p-values (`Pr>|t|`)
- Confidence intervals (`[0.025 0.975]`)

---

## A Note About Model Building

Building supervised learning models is a highly iterative process!

**Key Insights:**

- It is as much **art** as it is **science**
- It requires an understanding of both the business context and the machine learning method
- There is no absolute right or wrong model

The goal is to find a model that balances accuracy, interpretability, and practical usefulness for the business problem at hand.