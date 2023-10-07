# Ex-03 Univariate Analysis
## Aim:
To read the given data and perform the univariate analysis with different types of plots.

## Explanation:
Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.

## Algorithm:
### Step 01: 
Read the given data.

### Step 02:
Get the information about the data.

### Step 03
Remove the null values from the data.

### Step 04
Mention the datatypes from the data.

### Step 05
Count the values from the data.

## Program:
### Superstore CSV File:
```python
import pandas as pd
import numpy as np
import seaborn as sns
df=pd.read_csv('SuperStore.csv')
print(df)
df.head()
df.info()
df.dtypes
df['Postal Code'].value_counts()
sns.boxplot(x='Postal Code', data=df)
sns.countplot(x='Postal Code',data=df)
sns.distplot(df["Postal Code"])
df.describe()
```

### Diabetes CSV File:
```python
import pandas as pd
import numpy as np
import seaborn as sns
df = pd.read_csv("/diabetes.csv")
df
df.info()
df.isnull().sum()
df.dtypes
df.describe()
df['Glucose'].value_counts()
sns.boxplot(x="Glucose",data=df)
sns.countplot(x="Glucose",data=df)
sns.distplot(df['Glucose'])
sns.histplot(x="Glucose",data=df)
df.skew()
df.kurtosis()
```

### Employee Salary CSV File:
```python

import pandas as pd
df=pd.read_csv("/content/employeesal.csv")
df
df.info()
df.dtypes
df['Salary'].value_counts()
df.describe()
import seaborn as sns
sns.boxplot(x='Experience_Years',data=df)
sns.countplot(x="Experience_Years",data=df)
sns.distplot(df['Experience_Years'])
sns.histplot(x="Experience_Years",data=df)
df.skew()
sns.histplot(x='Salary',data=df)
sns.distplot(df['ID'])
df.kurtosis()
sns.boxplot(x='Salary',data=df)
sns.boxplot(x='Experience_Years',data=df)
```
## Output:
### Superstore Output:
https://user-images.githubusercontent.com/119393675/270012729-87fe1231-0142-4465-a675-bd57bcf82dfa.png
https://user-images.githubusercontent.com/119393675/270012753-da570c24-3faa-4abc-adb3-56ee3ae4c935.png
