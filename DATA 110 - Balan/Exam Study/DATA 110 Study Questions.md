# Quiz 1 Practice Problems

## Question 1

What is the result of this Python code?

```python
Text = "Hello World"
print(text.lower())
```

a. HELLO WORLD b. hello world c. Helloworld ===d. The code gives an error.===

---

## Question 2

If `x = 5` and `y = 10`, what will this code print?

```python
if x < 10 and y > 5:
    print("condition met")
```

**ANSWER:** 'condition met'

---

## Question 3

What does this code return?

```python
df.isna().sum()
```

a. Total number of rows in the dataframe 
===b. Number of missing values for each column in the dataframe ===
c. Number of non-missing values for each column in the dataframe 
d. Number of unique values for each column in the dataframe

---

## Question 4

In Pandas, `df.info()` can be used to generate:

a. Summary statistics for each numeric column 
===b. Data types and non-null counts for each column ===
c. Frequency counts for each categorical column

---

## Question 5

What is one function you could use to help you determine whether there are entries that have been miscoded or misspelled for a categorical column in a data frame?

**ANSWER:** df.value_counts()

---

## Question 6

Suppose that you run the code `df.head(3)`. What does this command return? How would the output change if we used `df.tail(3)` instead?

**ANSWER:**
df.head()

---

## Scenario: Retail T-Shirt Store Analysis

For the remaining questions, consider the following scenario:

A small chain of retail stores sells t-shirts featuring popular music artists (Taylor Swift, Beyonce, Drake, BTS, etc). Management wants to understand which artists sell the most, what sizes are the most popular, and how revenue is impacted by demographic factors (among other things).

### Data Dictionary

|Column Name|Column Description|
|---|---|
|transaction_id|Unique ID for each purchase|
|artist|Artist on the t-shirt|
|store|Store location (downtown, mall, online)|
|size|t-shirt size (S, M, L, XL)|
|gender|Gender of buyer (F, M, nonbinary)|
|age|Age of buyer|
|price|Price of t-shirt|
|units_sold|Number of shirts bought per transaction|
|revenue|Revenue (price x units_sold)|

Before beginning your analysis, you run `df.info()` and `df.head()`. This produces the following output:

![Screenshot of df.info() and df.head() output](media/image1.png)

---

## Question 7

How many rows are in the data set?

**ANSWER:**

---

## Question 8

Do any of the columns have missing values? How can you tell?

**ANSWER:**

---

## Question 9

Should artist be treated as nominal, ordinal, or interval?

**ANSWER:**

---

## Question 10

Should price be treated as nominal, ordinal, or interval?

**ANSWER:**

---

## Question 11

Should transaction_id be treated as nominal, ordinal, or interval?

**ANSWER:**

---

## Question 12

Based on the bar chart shown below, what is the mode of the distribution of shirt size?

a. Small (S) b. Medium (M) c. Large (L) d. Extra Large (XL)

![Bar chart of shirt size distribution](media/image2.png)

---

## Question 13

The owner of the store is considering a move to online-only. Based on the bar chart shown below, do you think that this is a good idea? Why or why not?

**ANSWER:**

![Bar chart of store location distribution](media/image3.png)

---

## Question 14

Which most closely describes the distribution of age?

a. Skewed to the Left b. Symmetric c. Skewed to the Right d. Bi-modal

![Histogram of customer age distribution](media/image4.png)

---

## Question 15

What would be the best measure of center for describing the distribution of price (mean, median or mode)? Why?

**ANSWER:**

![Histogram of sales price distribution](media/image5.png)

---

## Question 16

Consider the boxplot illustrating the distribution of sales price:

![Boxplot of sales price distribution](media/image6.png)

Which of the following statements is true of this distribution?

a. There are outliers present in the distribution. b. 50% of sales prices are greater than $25. c. 50% of the sales prices are less than $15. d. Both a and b.

---

## Question 17

The store owner is still considering a move to online only. He decides to compare the revenue from each store location to try to determine if there are any differences in the sales across the two brick and mortar stores and the online store. What conclusions can you reach based on the comparative boxplot below?

**ANSWER:**

![Comparative boxplot of revenue by store location](media/image7.png)