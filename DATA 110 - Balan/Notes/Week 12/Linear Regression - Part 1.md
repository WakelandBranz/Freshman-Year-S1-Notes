## Review: Scatterplots and Correlation

### Scatterplots

Scatterplots are graphical displays that show the relationship between two quantitative variables by plotting data points on a coordinate plane.

**Example Code (Python):**

```python
# Scatterplot of Sales Price vs Lot Area
plt.figure()
sns.scatterplot(data=df, x='LotArea', y='SalePrice')
plt.title('Lot Size (sf) vs Sales Price ($)')
plt.xlabel('Lot Size in Square Feet')
plt.ylabel('Sales Price ($)')
plt.show()
```

### What Are We Looking For?

When examining a scatterplot, ask yourself:

- Does there appear to be a relationship between the variables or do the points appear to be randomly scattered?
- Is the relationship linear?
    - Increasing?
    - Decreasing?
- Is there a nonlinear relationship?
- Are there any outliers or unusual features?

### Correlation ($r$)

**Correlation** measures the strength of the linear relationship between two quantitative variables.

**Key Properties:**

- Ranges from $-1$ to $1$
- The larger $|r|$ is, the stronger the linear relationship between the two variables
- Values of $r$ near zero indicate that there is no linear relationship between the two variables
- $r = 1$ or $r = -1$ indicates a perfect linear relationship
- The sign of $r$ tells you whether the relationship is positive (increasing) or negative (decreasing)
- Correlation is sensitive to outliers or unusual observations

### ⚠️ Important Warning

**Correlation does not imply causation!**

Just because two variables are correlated does not mean that one causes the other.

---

## Goals of Linear Regression Analysis

1. **Describe/understand** how a set of variables influences a numeric response variable
    
2. **Predict** the values of a numeric response variable when new data becomes available
    

---

## Terminology

### Response Variable

The variable that you want to predict. Also known as:

- Y-variable
- Dependent variable
- Target variable
- Output variable

### Predictor Variables

The variables that you will use to explain the response variable. Also known as:

- X-variables
- Independent variables
- Explanatory variables
- Features
- Inputs

---

## Equation of a Straight Line

$$y = b_0 + b_1x$$

Where:

- $b_0$ = **intercept** – the point where the line crosses the y-axis ($x=0$)
- $b_1$ = **slope** – the change in $y$ for a 1-unit change in $x$

---

## How Do We Estimate the Coefficients?

The coefficients are estimated using a method called **"Ordinary Least Squares."**

This method finds the line that minimizes the squared distance between all of the points and the regression line.

---

## Multiple Linear Regression

**Multiple Linear Regression** extends simple linear regression concepts to include several independent variables (predictors).

**When to use:**

- Useful when a single predictor model is inadequate for predicting the response variable.

**Form of the multiple regression model:**

$$y = b_0 + b_1x_1 + b_2x_2 + b_3x_3 + \ldots + b_kx_k$$

Where:

- $b_0$ is the **intercept** (value of $y$ when all $x$'s are equal to 0)
- The coefficients $b_1$ to $b_k$ describe the **change in $y$ for a 1-unit change in $x_i$ while holding all other x-values constant**

---

## Recall the Real Estate Example

### Scenario

You have been hired by a local real estate investor who is interested in understanding more about what factors are influencing the prices of homes in his area.

**Objectives:**

- Help set prices for homes that he is preparing to sell
- Help make decisions about which homes to buy
- Determine how to renovate the homes that he currently owns

**Data Context:** These data include homes that were sold between 2006 and 2010. You can assume that he is using these data to make decisions about real estate investments in that same time frame (not current day).

---

## Real Estate Example: Data Dictionary

|Variable Name|Variable Description|
|---|---|
|**Id**|Property's Unique Numeric Identifier|
|**SalePrice**|Sale Price ($) when the home was sold|
|**LotArea**|Area of the lot in square feet (SF)|
|**TotalBsmt**|Area of the basement in SF (0 if the home does not have a basement)|
|**1stFlrSF**|Total area of the 1st floor of the home in SF|
|**2ndFlrSF**|Total area of the 2nd floor of the home in SF (0 if the home doesn't have a 2nd floor)|
|**FullBath**|Total number of full bathrooms in the house|
|**HalfBath**|Total number of half bathrooms in the house|
|**BedroomAbvGr**|Total number of bedrooms in the house (excluding the basement)|
|**TotRmsAbvGr**|Total number of rooms in the house (excluding the basement)|
|**Fireplaces**|Total number of fireplaces in the house|
|**GarageCars**|Total number of cars that fit into the garage (0 if no garage)|
|**WoodDeckSF**|Total square footage of wooden deck (0 if home doesn't have a wooden deck)|
|**OpenPorchSF**|Total square footage of open porch (0 if home doesn't have an open porch)|
|**EnclosedPorch**|Total square footage of enclosed porch|
|**3SsnPorch**|Total square footage of three season sunroom|
|**ScreenPorch**|Total square footage of screened porch|
|**PoolArea**|Total square footage of outdoor pool|
|**LotConfig**|Location of the lot (Inside, FR3 (facing road on 3 sides), FR2 (facing road on 2 sides), CulDSac, corner)|
|**BldgType**|Type of home (1Fam, 2fmCon (unit in a condominium building), Duplex, Twnhs, TwnhsE (end unit townhouse))|
|**YearBuilt**|Year the home was built|
|**YearRemodAdd**|Year the home was remodeled (updated)|
|**Foundation**|Type of foundation the home is built on (BrkTil (brick), CBlock (concrete blocks), PConc (poured concrete), Slab, Stone, Wood)|
|**CentralAir**|Y = home has central air conditioning, N = home does not have central air conditioning|
|**KitchenQual**|Condition of the kitchen (Gd, Fa, Ex, TA)|
|**PavedDrive**|Y = driveway is paved, N = driveway is not paved, P = driveway is partially paved|
|**YrSold**|Year the home was last sold|

---

## Interpreting the Results

### OLS Regression Results

```
============================================================================
Dep. Variable:          SalePrice   R-squared:                       0.595
Model:                        OLS   Adj. R-squared:                  0.593
Method:            Least Squares   F-statistic:                     426.8
Date:              Tue, 28 Oct 2025   Prob (F-statistic):          4.57e-282
Time:                      16:44:04   Log-Likelihood:               -17885.
No. Observations:              1460   AIC:                         3.578e+04
Df Residuals:                  1454   BIC:                         3.581e+04
Df Model:                         5
Covariance Type:          nonrobust
============================================================================
                   coef    std err          t      P>|t|    [0.025      0.975]
----------------------------------------------------------------------------
const        -2.791e+04   6124.722     -4.557      0.000  -3.99e+04  -1.59e+04
GarageCars    3.878e+04   2133.976     18.173      0.000   3.46e+04   4.3e+04
1stFlrSF        66.7051      4.048     16.480      0.000     58.765     74.645
LotArea          0.6246      0.140      4.465      0.000      0.350      0.899
BedroomAbvGr  -773.5160   1761.803     -0.439      0.661  -4229.462   2682.430
FullBath       3.731e+04   2991.762     12.472      0.000   3.14e+04   4.32e+04
============================================================================
```

### Key Model Statistics

- **R-squared: 0.595** – The model explains 59.5% of the variation in sale price
- **Adj. R-squared: 0.593** – Adjusted for the number of predictors
- **F-statistic: 426.8** – Overall model significance test
- **Prob (F-statistic): 4.57e-282** – Extremely small p-value indicates the model is highly significant

---

## Interpreting the Slope

**The slope is the change in $y$ for a 1-unit change in $x$ (holding everything else constant)**

### Example: Garage Renovation Decision

**Scenario:** Suppose that you are thinking about renovating your garage to fit one additional car. The cost of the renovation is estimated to be $25,000. You only want to do the renovation if you could recoup the cost when you sell the house. Should you do the renovation?

**Analysis:**

- Slope for GarageCars is $3.878 \times 10^4$ or **$38,780**
- This means that you would expect a **$38,780 increase in sales price** if you increased the number of cars that can fit into the garage by 1

**Conclusion:** Since the expected increase in sale price ($38,780) exceeds the renovation cost ($25,000), you should do the renovation because you would recoup the investment and gain an additional $13,780 in value.

---

## Making a Prediction

### Example Home

Suppose that you are interested in purchasing a house that has:

- 2-car garage
- 1100 square feet on the first floor
- Lot area of 10,000 square feet
- 3 bedrooms in the main floor of the house
- 2 full bathrooms

**How much should you expect to pay?**

### Calculation

Using the regression equation:

$$\text{SalePrice} = b_0 + b_1(\text{GarageCars}) + b_2(\text{1stFlrSF}) + b_3(\text{LotArea}) + b_4(\text{BedroomAbvGr}) + b_5(\text{FullBath})$$

Substituting the values:

$$\begin{align} \text{SalePrice} &= -27,910 \ &\quad + (38,780 \times 2) \ &\quad + (66.71 \times 1,100) \ &\quad + (0.6246 \times 10,000) \ &\quad - (773.516 \times 3) \ &\quad + (37,310 \times 2) \end{align}$$

$$\text{SalePrice} = -27,910 + 77,560 + 73,381 + 6,246 - 2,321 + 74,620$$

$$\text{SalePrice} = $201,577$$

**Expected Price: $201,577**

---

## Warnings!

### 1. Correlation Does Not Imply Causation

Just because two variables are related in a regression model does not mean that one causes the other. There may be confounding variables or the relationship may be coincidental.

### 2. Beware of Extrapolation!

**Extrapolation:** Using the regression model to make predictions for values of X outside of the range of X-values used to train the model.

### Example: GMC Truck Prices

Consider a regression model predicting truck prices based on age:

**Left plot (Training Data):**

- Age range: 5-15 years
- Price range: $5,000-$25,000
- Clear negative relationship

**Right plot (With Extrapolation):**

- Age range extended to 0-40 years
- Shows how predictions become unreliable outside the training range
- The model may predict negative prices for very old trucks or unrealistic prices for new trucks

**Key Takeaway:** Only use regression models to make predictions within the range of the data used to build the model. Predictions outside this range (extrapolation) can be highly unreliable and misleading.

---

## Summary

### Linear Regression Fundamentals

1. Linear regression models the relationship between a response variable and one or more predictor variables
2. The equation of a straight line is $y = b_0 + b_1x$
3. Multiple linear regression extends this to: $y = b_0 + b_1x_1 + b_2x_2 + \ldots + b_kx_k$

### Interpretation

- The intercept ($b_0$) is the predicted value when all predictors are zero
- Each slope coefficient represents the change in the response for a 1-unit increase in that predictor, holding all other predictors constant
- R-squared measures the proportion of variance explained by the model

### Best Practices

- Always examine scatterplots before building models
- Remember: correlation ≠ causation
- Never extrapolate beyond the range of your data
- Check model assumptions and diagnostics (covered in later modules)

### Real-World Applications

- Predicting home prices based on features
- Understanding which factors most influence outcomes
- Making data-driven business decisions
- Evaluating the return on investment for improvements