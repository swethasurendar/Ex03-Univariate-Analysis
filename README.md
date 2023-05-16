# Ex03-Univariate-AnalysisAim
# Aim 
To read the given data and perform the univariate analysis with different types of plots

# Explanation
Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.

# Algorithm
Step1
Read the given data.

Step2
Get the information about the data.

Step3
Remove the null values from the data.

Step4
Mention the datatypes from the data.

Step5
Count the values from the data.

Step6
Do plots like boxplots,countplot,distribution plot,histogram plot.

# Program
```
# Developed by        : SWETHA
# Registration Number : 212221220054
import pandas as pd
import numpy as np
import seaborn as sns

df=pd.read_csv('superstore.csv')
df

df.head()
df.info()
df.describe()
df.isnull().sum()

df.dtypes

df['Postal Code'].value_counts()

sns.boxplot(x='Postal Code', data=df)
sns.countplot(x='Postal Code',data=df)
sns.distplot(df["Postal Code"])
sns.histplot(x='Postal Code',data=df)
```
# OUTPUT

# DATA
![image](https://github.com/swethasurendar/Ex03-Univariate-Analysis/assets/133625914/943c56c6-828d-4f2f-85d7-e5fb96b1bb83)
# DATA HEAD
![image](https://github.com/swethasurendar/Ex03-Univariate-Analysis/assets/133625914/f4c5a0ed-20a4-4cdf-b0b1-23fb4eaf9b4d)
# DATA INFORMATION
![image](https://github.com/swethasurendar/Ex03-Univariate-Analysis/assets/133625914/99b2e591-60dd-424e-8c00-ce2b09ce2698)
# DATA DESCRIBE
![image](https://github.com/swethasurendar/Ex03-Univariate-Analysis/assets/133625914/e33b02f9-dd57-401e-a825-1afdff06405e)
# DATA NULL VALUES
![image](https://github.com/swethasurendar/Ex03-Univariate-Analysis/assets/133625914/323c6511-860c-4728-ac81-6665781ffdce)
# DATA'S VALUECOUNT
![image](https://github.com/swethasurendar/Ex03-Univariate-Analysis/assets/133625914/d072f3dd-532e-49cf-98dd-1f210103753b)
# BOXPLOT
![image](https://github.com/swethasurendar/Ex03-Univariate-Analysis/assets/133625914/c5f1e312-ca0e-4455-b291-b2a54aa382c5)
# COUNTPLOT
![image](https://github.com/swethasurendar/Ex03-Univariate-Analysis/assets/133625914/dd49966d-38cb-46ad-b371-bd91a8341275)
# DISTRIBUTION PLOT
![image](https://github.com/swethasurendar/Ex03-Univariate-Analysis/assets/133625914/6810c1bd-172d-49ce-858d-480c3dca17df)
# HISTOGRAM PLOT
![image](https://github.com/swethasurendar/Ex03-Univariate-Analysis/assets/133625914/6ebcf9a4-0b60-4381-9c63-245a64eef9d0)
# Result
Thus we have read the given data and performed the univariate analysis with different types of plots.






