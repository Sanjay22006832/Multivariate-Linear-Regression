# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
import pandas as pd

### Step2
Read the csv file
### Step3
Get the values of x and y variables.

### Step4
Create the linear regression model and fit.

### Step5
Predict the CO2 emission of a car where the weight is 3300kg, and the vlume is 1300cm3.

### Step6:
Print the predicted output.

## Program:
```
Program to implement multivariate linear regression and predict the output.
Developed by: M. Sanjay
Register number: 212222240090

import pandas as pd
from sklearn import linear_model
df=pd.read_csv("cars (1).csv")
a=df[["Weight","Volume"]]
b=df[["CO2"]]
regr=linear_model.LinearRegression()
regr.fit(a,b)
print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)
print("Amount:",regr.predict([[3300,1300]]))
```
## Output:

![image](https://github.com/Sanjay22006832/Multivariate-Linear-Regression/assets/119830477/19fe3cfa-e543-4345-9499-c25f8bb959fe)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
