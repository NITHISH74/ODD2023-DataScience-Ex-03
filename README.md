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
![image](https://github.com/NITHISH74/ODD2023-DataScience-Ex-03/assets/94164665/f86a031c-d315-470f-b3ee-1b73206326dc)
![image](https://github.com/NITHISH74/ODD2023-DataScience-Ex-03/assets/94164665/29a13092-152f-45a6-afac-f808dc4f618b)
![image](https://github.com/NITHISH74/ODD2023-DataScience-Ex-03/assets/94164665/bcf37d33-2839-4fc6-a2e7-cf33e9878167)
![image](https://github.com/NITHISH74/ODD2023-DataScience-Ex-03/assets/94164665/1e311fab-8dc0-403a-98e3-49ef783dc680)
![image](https://github.com/NITHISH74/ODD2023-DataScience-Ex-03/assets/94164665/44ba03a6-6e93-4994-abf7-40a868de2c11)

### Diabetes Output:
![image](https://github.com/NITHISH74/ODD2023-DataScience-Ex-03/assets/94164665/39132738-0277-4457-895d-be5b92fc1e43)
![image](https://github.com/NITHISH74/ODD2023-DataScience-Ex-03/assets/94164665/a2a5f70f-c402-4e12-99c7-027a5d2b6872)
![image](https://github.com/NITHISH74/ODD2023-DataScience-Ex-03/assets/94164665/6ab15ba2-070f-45d1-b9cc-9bf1c443d130)
![image](https://github.com/NITHISH74/ODD2023-DataScience-Ex-03/assets/94164665/fdbe136a-7d46-451b-acf6-53f54b4c653a)
![image](https://github.com/NITHISH74/ODD2023-DataScience-Ex-03/assets/94164665/e6e03e4c-4c18-445a-b668-734ea0e8956f)
![image](https://github.com/NITHISH74/ODD2023-DataScience-Ex-03/assets/94164665/53f655c7-b76f-4383-96a0-f864c851728d)

### Employee Salary Output:
![image](https://github.com/NITHISH74/ODD2023-DataScience-Ex-03/assets/94164665/af33c8af-5c69-45ba-b3a5-9ba47d077474)
![image](https://github.com/NITHISH74/ODD2023-DataScience-Ex-03/assets/94164665/34a24385-ec15-4b2f-b088-6edc5b00b523)
![image](https://github.com/NITHISH74/ODD2023-DataScience-Ex-03/assets/94164665/0b28f01a-8aad-48e3-8749-c8ac9ac0f102)
![image](https://github.com/NITHISH74/ODD2023-DataScience-Ex-03/assets/94164665/267cf2d6-36e6-4cd0-9e35-2e42b6f7ff93)
![image](https://github.com/NITHISH74/ODD2023-DataScience-Ex-03/assets/94164665/1d13fc96-ccd5-49c8-877f-2ccfc7e11f50)
![image](https://github.com/NITHISH74/ODD2023-DataScience-Ex-03/assets/94164665/24ac1f19-ba61-4898-9c5e-5b3fa317e4ed)
![image](https://github.com/NITHISH74/ODD2023-DataScience-Ex-03/assets/94164665/cd36a4ce-0e4d-42e3-a80c-a1fd04217b5e)
![image](https://github.com/NITHISH74/ODD2023-DataScience-Ex-03/assets/94164665/0ef2ae1a-b0b0-4565-bb84-a93f6f6ef80a)

## Result:
Hence the given CSV File was verified successfully with the help of the Univariate Analysis technique.



