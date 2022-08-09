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

sum()

alcohol.cumsum()

alcohol.cumprod()

# 56 Pairwise Differences with diff()

# 57 Iteration Series

for i, v in mini_alc.items():
    print(f'Index:{i}, value:{v}')

# 58 Filtering: filter(), where(), and mask()

## filter on index:

alcohol.filter(regex='^V') 

alcohol.filter(like='stan') **<- like in SQL>**

## fileter on values:

alcohol.get(alcohol > 200)

def gt200(x): return x > 200

alcohol[gt200]

### replace with corresponding value when condition is FALSE

alcohol.where(lambda x: x > 200, other='Too small.')

alcohol.where(lambda x:x>200, other=pd.NA) <-default  NaN>

alcohol.where(lambda x:x>200).dropna()

### replace with corresponding value when condition is TRUE

alcohol.where(lambda x:x<=200).dropna()

alcohol.mask(lambda x:x>200).dropna()

# 59 Transforming with update(), apply(), map()

## Spot change

alcohol.update(pd.Series(data=[200,20], index=['Albania','Andorra']))

## global change

alcohol.apply(lambda x:x**2)

alcohol.apply(np.square) <-vectorized operations >

https://www.pythonlikeyoumeanit.com/Module3_IntroducingNumpy/VectorizedOperations.html

def multiply_by_self(x): return x*x

alcohol.apply(multiply_by_self)

## substituting each values in a Series with another values

### in siple transformations apply & map is the same for more advanced transformation use apply

# 60 Sill Challenge

pip install scipy

https://stackoverflow.com/questions/24761998/pandas-compute-z-score-for-all-columns

https://pandas.pydata.org/docs/user_guide/visualization.html




