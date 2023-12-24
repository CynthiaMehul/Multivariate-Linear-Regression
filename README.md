# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import pandas module to solve for multivariate linear regression.	

### Step2
From sklearn import	linear_model.	

### Step3
Open the file cars and get input for weight and	volume to find density of CO2.	

### Step4
Print coefficients, intercept and amount.	

### Step5
End Program.

## Program:
```
#To implement multivariate linear regression
#Developed by: Cynthia Mehul J
#Register number:23009725

import pandas as pd
from sklearn import linear_model
df=pd.read_csv('cars.csv')
x=df[['Weight','Volume']]
y=df[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(x,y)
print('coefficients:',regr.coef_)
print('Intercept:',regr.intercept_)
print("Amount:",regr.predict([[3300,1300]]))
```
## Output:
![label](/Program.jpg)

![label](/Output.jpg)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.