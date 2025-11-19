## Exam 1 Quiz - 20 Questions

## Question 1

What data scale should be used for customer satisfaction ratings (Very Unsatisfied, Unsatisfied, Neutral, Satisfied, Very Satisfied)?

a. Nominal b. ===Ordinal=== c. Interval d. Boolean

---

## Question 2

Which Python data type would be most appropriate for storing the value `3.14159`?

a. int b. ===float=== c. bool d. str

---

## Question 3

What does `df.describe()` return?

a. Data types for each column 
===b. Summary statistics for numeric columns ===
c. Frequency counts for categorical columns 
d. The first 5 rows of the dataframe

**ANSWER:**

---

## Question 4

Write the correct syntax to find the maximum value in a column called `revenue` in a dataframe called `sales`.

**ANSWER:**

sales['revenue'].max()

---

## Question 5

What will this code print?

```python
score = 85

if score >= 90:
    print("A")
elif score >= 80:
    print("B")
elif score >= 70:
    print("C")
else:
    print("F")
```

a. A b. ===B=== c. C d. F

---

## Question 6

Which function would you use to find all unique values and their frequencies in a categorical column?

a. df.unique() b. df.count() c. ===df.value_counts()=== d. df.sum()

---

## Question 7

What does the following code accomplish?

```python
df.groupby('department').salary.mean()
```

**ANSWER:**
Gets the mean salary of all of the departments

---

## Question 8

According to best practices for data visualization, which of the following should you do?

a. Use as many colors as possible 
===b. Include gridlines for precision ===
c. Maximize the data-to-ink ratio 
d. Use small fonts to fit more information

---

## Question 9

What is the mode of a distribution?

a. The average value b. The middle value ===c. The most frequently occurring value=== d. The range of values

---

## Question 10

Which type of chart is most appropriate for visualizing the distribution of a single categorical variable?

a. Scatterplot b. Histogram c. ===Bar chart=== d. Line chart

---

## Question 11

In a boxplot, what does the box itself represent?

a. The minimum and maximum values b. The interquartile range (IQR) c. All outliers in the data d. The mean ± standard deviation

**ANSWER:**

---

## Question 12

If Q1 = 25 and Q3 = 75, what is the IQR?

a. 25 b. 50 c. 75 d. 100

---

## Question 13

What percentage of data falls within the interquartile range?

a. 25% b. 50% c. 75% d. 100%

---

## Question 14

Which type of plot is best for examining the relationship between two numeric variables?

a. Bar chart b. Pie chart c. Scatterplot d. Histogram

---

## Question 15

What does `df.isna().sum()` return?

**ANSWER:**

---

## Question 16

A distribution where most values are concentrated on the left with a tail extending to the right is described as:

a. Skewed to the left b. Skewed to the right c. Symmetric d. Bimodal

---

## Question 17

Which data scale is appropriate for zip codes?

a. Nominal b. Ordinal c. Interval d. Ratio

---

## Question 18

What is true about Python's `float` data type?

a. It can only represent whole numbers b. It always has unlimited precision c. It has limited precision of 15-16 decimal places d. It cannot be used in mathematical operations

---

## Question 19

When comparing a categorical variable to a numeric variable, which visualization should you use?

a. Scatterplot b. Comparative boxplots c. Heatmap d. Pie chart

---

## Question 20

What is the difference between `df.head()` and `df.tail()`?

**ANSWER:**

---

## Answer Key (For Instructor Use)

1. b
2. b
3. b
4. `sales.revenue.max()` or `sales['revenue'].max()`
5. b
6. c
7. Calculates the average salary for each department
8. c
9. c
10. c
11. b - The box represents the IQR, containing the middle 50% of the data between Q1 and Q3
12. b
13. b
14. c
15. The number of missing values for each column in the dataframe
16. b
17. a
18. c
19. b
20. `df.head()` returns the first n rows (default 5), while `df.tail()` returns the last n rows (default 5)