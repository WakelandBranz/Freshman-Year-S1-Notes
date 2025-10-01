### Quiz 1 Alternative Practice Problems

### Python and Pandas Basics

### Question 1

What is the result of this Python code?

```python
name = "DATA SCIENCE"
print(name.lower())
```

- [ ] a. DATA SCIENCE
- [x] b. data science
- [ ] c. Data Science
- [ ] d. The code gives an error

---

### Question 2

If `a = 15` and `b = 20`, will this code print anything? If so, what?

```python
if a > 10 or b < 15:
    print("condition is true")
```

**Answer:**
This will print 'condition is true'

---

### Question 3

What does the following Pandas code return?

```python
df.describe()
```

- [ ] a. Total number of rows in the dataframe
- [x] b. Summary statistics (mean, std, min, max, quartiles) for numeric columns
- [ ] c. Data types for each column
- [ ] d. The first 5 rows of the dataframe

---

### Question 4

Which Pandas function would you use to see the frequency of values in a categorical column?

- [ ] a. df.head()
- [ ] b. df.info()
- [x] c. df.value_counts()
- [ ] d. df.describe()

---

### Question 5

You want to check if there are any duplicate values in the 'transaction_id' column of your dataframe. What function could you use?

**Answer:**
df.duplicated()

---

### Question 6

Suppose you run the code `df.shape`. What information does this return? How is this different from `df.info()`?

**Answer:**

---

## T-Shirt Sales Scenario

**Context:** A small chain of retail stores sells t-shirts featuring popular music artists (Taylor Swift, Beyonce, Drake, BTS, etc). Management wants to understand which artists sell the most, what sizes are the most popular, and how revenue is impacted by demographic factors.

**Dataset columns:**

- transaction_id: Unique ID for each purchase
- artist: Artist on the t-shirt
- store: Store location (downtown, mall, online)
- size: t-shirt size (S, M, L, XL)
- gender: Gender of buyer (F, M, nonbinary)
- age: Age of buyer
- price: Price of t-shirt
- units_sold: Number of shirts bought per transaction
- revenue: Revenue (price x units_sold)

**Dataset info:** 200 rows, 9 columns, no missing values

---

### Question 7

If you wanted to find out which artist's t-shirts generate the most total revenue, what type of analysis would you perform?

**Answer:**
Group by artists and sum revenue

---

### Question 8

The 'gender' column contains values: F, M, and nonbinary. Should this be treated as nominal, ordinal, or interval?

**Answer:**
Nominal

---

### Question 9

The 'size' column contains values: S, M, L, XL. Should this be treated as nominal, ordinal, or interval?

**Answer:**

---

### Question 10

Based on this data showing revenue by artist:

- Beyonce: $120,000
- Drake: $100,000
- Taylor Swift: $135,000
- BTS: $60,000

Which artist generates the most revenue?

- [ ] a. Beyonce
- [ ] b. Drake
- [ ] c. Taylor Swift
- [ ] d. BTS

---

### Question 11

A histogram shows the distribution of units sold per transaction. Most transactions (about 120) involve 1 unit, about 80 involve 2 units, about 40 involve 3 units, and about 20 involve 4+ units. What can you conclude?

- [ ] a. Most transactions involve purchasing 1 shirt
- [ ] b. Most transactions involve purchasing 2 shirts
- [ ] c. The distribution is uniform
- [ ] d. The distribution is bimodal

---

### Question 12

Looking at a histogram of customer age, the distribution shows the highest frequencies around ages 25-35, with the tail extending toward younger ages (15-20). This distribution is:

- [ ] a. Right-skewed (positively skewed)
- [ ] b. Left-skewed (negatively skewed)
- [ ] c. Approximately symmetric
- [ ] d. Bimodal

---

### Question 13

A histogram of revenue per transaction shows most values clustered between $15-$75, with a few extreme values at $150-$200. Would the mean or median be a better measure of center? Why?

**Answer:**

---

### Question 14

A boxplot comparing price by gender shows all three groups (F, M, Nonbinary) have similar medians around $20 and similar box sizes, with one outlier in the female category at $50. Which statement is TRUE?

- [ ] a. There is high variability in prices across all gender groups
- [ ] b. The median price is similar across all three gender groups
- [ ] c. Male customers pay significantly more on average
- [ ] d. There are no outliers in the data

---

### Question 15

A boxplot comparing revenue across the three store locations (Downtown, Mall, Online) shows that all three have similar medians around $50, similar IQRs, and a few high outliers in each. What business conclusion might you draw?

**Answer:**

---

### Question 16

If you calculate `df['price'].mean()` and get 23.45, and `df['price'].median()` and get 19.50, what does this tell you about the distribution of price?

**Answer:**

---

### Question 17

Management wants to know: "Do customers buy more units per transaction when shopping online versus in-store?" What type of visualization would be most appropriate to answer this question?

- [ ] a. A histogram of units_sold
- [ ] b. A comparative boxplot of units_sold by store location
- [ ] c. A bar chart of store locations
- [ ] d. A scatter plot of price versus units_sold

---

## Notes Section

Use this space for any additional notes or calculations: