# Ex03-Univariate-Analysis
# Aim:
To read the given data and perform the univariate analysis with different types of plots.

# Theory:
Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.

# Algorithm:
## Step 1:
Read the given data.
## Step 2:
Get the information about the data.

## Step 3:
Remove the null values from the data.

## Step 4:
Mention the datatypes from the data.

## Step 5:
Count the values from the data.

## Step 6:
Do plots like boxplots,countplot,distribution plot,histogram plot.

# Program:
```
Program developed by : Shrruthilaya G
Register number : 212221230097

import pandas as pd
import numpy as np
import seaborn as sns

data=pd.read_csv('SuperStore.csv')
data

data.head()

data.info()

data.describe()

data.isnull().sum()

data.dtypes

data['Postal Code'].value_counts()

sns.boxplot(x='Postal Code', data=data)

sns.countplot(x='Postal Code',data=data)

sns.distplot(data["Postal Code"])

sns.histplot(x='Postal Code',data=data)
```
# Output:
## Dataset:
![](dataset.png)

## Head data:
![](head.png)

## Dataset Information:
![](info.png)

## Data Description:
![](describe.png)

## Null data:
![](null.png)

## Datatype:
![](dtypes.png)
## Value counts:
![](valuecounts.png)

## Box plot:
![](boxplot.png)

## Count plot:
![](countplot.png)

## Distribution plot:
![](distplot.png)

## Histogram plot:
![](histplot.png)

# Result:
Thus, we have read the given data and performed the univariate analysis with different types of plots.