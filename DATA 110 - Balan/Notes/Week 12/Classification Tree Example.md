**Predicting Churn at a Telecommunications Company**

---

## Telecommunication Churn

A large telecommunications company is concerned because the percentage of customers who leave the company for another service provider is too high.

**Objective:** Identify customers who are likely to churn (switch wireless service providers) when their contract ends in order to develop a strategy for retaining valuable customers.

**Note:** This example uses the data and code from Lab 8.

---

## Data Dictionary

|Variable Name|Description|
|---|---|
|State|State of Residence|
|Account Length|Number of weeks customer has been with the company|
|Area Code|3 digit area code|
|Phone|7 digit phone number|
|Int'l Plan|Does the customer have an international plan? Yes/No|
|VMail Plan|Does the customer have a voicemail plan? Yes/No|
|Vmail Message|Number of voice mail messages received per month|
|Day Mins|Daytime calling minutes used per month|
|Day Calls|Number of daytime calls per month|
|Day Charge|Daytime calling charges per month in USD|
|Eve Mins|Evening calling minutes used per month|
|Eve Calls|Number of evening calls per month|
|Eve Charge|Evening calling charges per month in USD|
|Night Mins|Nighttime calling minutes used per month|
|Night Calls|Number of nighttime calls per month|
|Night Charge|Nighttime calling charges per month in USD|
|Intl Mins|International calling minutes used per month|
|Intl Calls|Number of international calls per month|
|Intl Charge|International calling charges per month in USD|
|CustServ Calls|Number of customer service calls per month|
|Churn?|1 if the customer switched providers, 0 otherwise|

---

## Data Preparation

1. **Drop unnecessary variables:**
    
    - Drop State, Area Code, and Phone Number
    - Reason: State and Area Code are categorical variables with many levels
    - Area Code + Phone Number is a unique identifier
2. **Check for missing values:**
    
    - No missing values in the data set!
3. **Recode categorical variables:**
    
    - Int'l Plan and VMail Plan are categorical variables coded as "yes" and "no"
    - Recode to 0 and 1 (numeric) for modeling
4. **Separate data:**
    
    - Separate data into X and Y data frames
5. **Split data:**
    
    - Split data into training and test sets

---

## Code: Splitting Data

```python
# split the data into training and testing sets
X = df.drop(['Churn?'], axis=1)

y = df['Churn?']
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.3, random_state=42)
```

---

## Fit a Classification Tree to the Training Data

### Code

```python
# create an instance of a decision tree classifier using default values
dt = DecisionTreeClassifier(max_depth = 25, min_samples_leaf=10, ccp_alpha = 0.001)

# fit the model to the training data
dt.fit(X_train, y_train)
```

### Parameters

- **max_depth:** Determines the maximum number of levels for the tree. Smaller values help to prevent overfitting.
    
    - Default value = None
- **min_samples_leaf:** Determines the minimum number of observations that must remain in a leaf after splitting. If a split leaves fewer than this number of observations, the split cannot be performed. Larger values help to prevent overfitting.
    
    - Default value = 1
- **ccp_alpha:** The cost complexity parameter and can be used for post-pruning the tree to help prevent overfitting. Larger values yield a smaller tree.
    
    - Default value = 0

---

## Interpreting the Tree

### Tree Structure Overview

The classification tree starts with the root node and branches based on various feature conditions. Each node in the tree contains:

- The splitting condition (e.g., $\text{Day Mins} \leq 263.55$)
- **gini:** The Gini impurity measure (lower is better)
- **samples:** The number of observations in that node
- **value:** The count of [class 0, class 1] observations
- **class:** The predicted class (0 = not churn, 1 = churn)

### Root Node Analysis

**Node: $\text{Day Mins} \leq 263.55$**

- gini = 0.249
- samples = 2333
- value = [1993.0, 340.0]
- class = 0

This is the first split in the tree. If a customer uses ≤ 263.55 daytime minutes per month, go left (True); otherwise, go right (False).

### Key Decision Paths

#### Left Branch (Day Mins ≤ 263.55):

**Node: $\text{CustServ Calls} \leq 3.5$**

- gini = 0.204
- samples = 2174
- value = [1923, 251]
- class = 0

Most customers with lower daytime minutes and fewer customer service calls do not churn.

**Further split:** $\text{Day Mins} \leq 165.85$

- Smaller subsets split based on additional features
- Nodes with very low gini values indicate pure or nearly pure classifications

#### Right Branch (Day Mins > 263.55):

**Node: $\text{VMail Plan} \leq 0.5$**

- gini = 0.493
- samples = 159
- value = [70, 89]
- class = 1

Customers with higher daytime minutes and no voicemail plan are more likely to churn.

**Further splits:**

- $\text{Eve Mins} \leq 184.65$
- $\text{Eve Charge} \leq 12.665$
- $\text{Night Calls} \leq 119.5$

### Color Coding in Tree Visualization

- **Orange nodes:** Predicted class = 0 (not churn)
- **Blue nodes:** Predicted class = 1 (churn)
- **Lighter shades:** Lower Gini impurity (more confident predictions)
- **Darker shades:** Higher Gini impurity (less confident predictions)

---

## Making a Prediction

### Example Customer Profile

Consider a customer with the following characteristics:

- Has a voicemail plan and an international plan
- Did not call customer service
- Uses 150 daytime minutes per month
- Has no international calls and no international charges

### Prediction Path Through the Tree

1. **Root Node:** $\text{Day Mins} \leq 263.55$ → **True** (150 ≤ 263.55)
    
    - Go left
2. **Node:** $\text{CustServ Calls} \leq 3.5$ → **True** (0 ≤ 3.5)
    
    - Go left
3. **Node:** $\text{Int'l Plan} \leq 0.5$ → **False** (has international plan = 1)
    
    - Go right
4. **Node:** $\text{Intl Charge} \leq 3.535$
    
    - Since there are no international charges (0 ≤ 3.535) → **True**
    - Go left
5. **Node:** $\text{Intl Calls} \leq 2.5$
    
    - Since there are no international calls (0 ≤ 2.5) → **True**
    - Go left
6. **Leaf Node:**
    
    - gini = 0.0
    - samples = 35
    - value = [0, 35]
    - **class = 1** (churn)

### Prediction Result

This customer is predicted to **churn** (class = 1), as they end up in a leaf node where all 35 samples churned.

---

## Key Takeaways

1. **Most important features for predicting churn:**
    
    - Day Mins (daytime minutes)
    - CustServ Calls (customer service calls)
    - VMail Plan (voicemail plan)
    - Int'l Plan (international plan)
    - Eve Mins (evening minutes)
2. **High-risk churn indicators:**
    
    - High daytime minutes usage
    - No voicemail plan
    - Multiple customer service calls
    - Having an international plan with low usage
3. **Low-risk churn indicators:**
    
    - Moderate daytime minutes usage
    - Few or no customer service calls
    - Having a voicemail plan
4. **Model interpretation:**
    
    - The tree provides clear, interpretable rules for classifying customers
    - Each path from root to leaf represents a specific customer profile
    - Leaf nodes with low gini values (near 0) indicate confident predictions