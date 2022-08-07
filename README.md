# The-ultimate-pandas-bootcamp-advanced-python-data-analysis
 https://nordea.udemy.com/course/the-ultimate-pandas-bootcamp-advanced-python-data-analysis/


# 25

iloc => integer loc => indexing by position
loc => location => indexing by label

# 26 - Using Callables with .loc and .iloc

lambda <-- anonimus function https://www.programiz.com/python-programming/anonymous-function

# 27 Seleting with .get()

# 28 Selection Recap

# 29 Skill challenge

https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.Series.equals.html

# 30 solutions

# 33 Reading data from csv

# 34 Series Sizing With .size .shape ANd len()

https://www.programiz.com/python-programming/methods/list/reverse

https://pbpython.com/pandas_dtypes.html

# 36 count() method

# 37 Accessing and counting NA's

## Pandorable <-- adorable and involving pandas

alcohol.isna().sum() == alcohol.isnull().sum()

# 38 BONUS: Another Approach

# 39 The Other Side: notnull() and notna()

# 40 BONSU: Booleans are literally number in Python

# 41 Skill Challenge

# 43 Dropping and filling NAs

# 44 Descriptice statistic

https://en.wikipedia.org/wiki/Quantile

alcohol.describe()

# 45 Describe() Method

from math import sqrt
sqrt()

# 46 mode() and value_counts()

alcohol.value_counts(normalize=True).head(n=17)

# 47: idxmax() & idxmin()

# 48 Sorting with sort_values()

alcohol.sort_values(ascending=False, na_position='first')

**alcohol.sort_values(ascending=False, na_position='last', kind='quicksort').head(n=1) <-- best one**

alcohol.sort_values(ascending=False, na_position='first', kind='mergesort').head(n=1)

alcohol.sort_values(ascending=False, na_position='first', kind='heapsort').head(n=3)

# 49 nlargest() and nsmallest()

# 50 Sorting with sort_index()

# 51 Skill Challenge

## 52 Solution

# 53 basic math Series arithmetics and fill_value()

# 54 Bonus: Calculating Varaince and Standard Deviation

# 55 Cumulative Operations


