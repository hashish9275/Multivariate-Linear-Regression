# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:

### Step1
Import panda module as pd
## Step 2:
Import linear model from sklearn
## Step 3:
Read the file cars.csv
## Step 4:
Assign the values for x and y as required
## Step 5:
Create the linearRegression model and predict the output

## Program:
```
'''
Programmed by: K.R.Hashish Vidya Sagmar
Register number: 212222230047
'''
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("cars.csv")
a=df[['Weight','Volume']]
b=df[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(a,b)
print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)
print("Amount:",regr.predict([[3300,1300]]))
```
## Output:
![image](https://github.com/hashish9275/Multivariate-Linear-Regression/assets/118707521/5f07e129-2d61-47a0-84e3-b6b6d5c4b2ac)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
