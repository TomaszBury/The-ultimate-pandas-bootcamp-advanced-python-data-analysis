String parse time:

`datetime.strptime()`

[Formating](https://docs.python.org/3/library/datetime.html#strftime-and-strptime-format-codes) <-- The following is a list of all the format codes that the 1989 C standard requires, and these work on all platforms with a standard C implementation.

```python
from dateutil import parser
parser.parse('22 april 2068 at 4pm and 17 minutes 20 seconds')
```

[TimeStamp](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.Timestamp.html) <-- doc

```python
pd.Timestamp('4/7/1776')
pd.to_datetime('4/7/1776',dayfirst=True)
```