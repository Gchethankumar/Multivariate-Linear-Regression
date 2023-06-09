# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step 1:

Import panda module as pd
### Step 2:

Import linear model from sklearn
### Step 3:

Read the file cars.csv
### Step 4:

Assign the values for x and y as required
### Step 5:

Create the linearRegression model and predict the output
## Program:
```
'''
Programmed by: G.Chethan kumar
Register number: 212222240022
'''
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("cars (1).csv")
a=df[['Weight','Volume']]
b=df[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(a,b)
print("coefficient",regr.coef_)
print("Intercept:",regr.intercept_)
print("Amount:",regr.predict([[3300,1300]]))
```
## Output:

![Screenshot 2023-06-09 190759](https://github.com/Gchethankumar/Multivariate-Linear-Regression/assets/118348224/6618c304-fb2f-4813-8b8e-b8a6114bf2a8)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
