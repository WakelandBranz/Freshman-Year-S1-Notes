##### Imputation - Replacement/removal of missing values

##### Copy and drop useless data into a separate 'dataframe' variable
```python
dataframe_copy = dataframe.copy() # copy dataframe for future usage

dataframe_copy.dropna() # drops ALL entries with missing data
```

```python
# fill missing data with junk filler data and get the mean of all numeric columns
df_filled = df.fillna(df.mean(numeric_only=True))

# print data of filled dataframe
df_filled.info()
```