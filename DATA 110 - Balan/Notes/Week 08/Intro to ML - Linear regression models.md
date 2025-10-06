#### Remember what r represents (correlation)!
 - r = 1
	 - Linear positive relationship
- r = -1
	- Linear negative relationship
- **Just describes the linearity of the data.**

#### df.corr() shows correlation between two data points (r value)

#### Creating a Correlation Matrix in Python
```Python
# Drop ordinal and nominal data, leaving only interval data
columns_to_drop = ['Id', 'Yearbuilt', 'YearRemodAdd', 'YrSold']
correlation_matrix = df.drop(columns = columns_to_drop).select_dtypes(include='number').corr()
```