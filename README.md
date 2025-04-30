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

Get the value of X and Y variables.

### Step4

Create the linear regression model and fit.
### Step5

Predict the CO2 emission of a car where the weight  is 2300kg and the volume is 1300cm cube.

## Program:
```
Developed by: Pavithra K
Register number: 212224240112


import pandas as pd 
from sklearn import linear_model 
df=pd.read_csv("car (1).csv") 
x=df[['Weight', 'Volume']] 
y=df['CO2'] 
regr=linear_model.LinearRegression() 
regr.fit(x,y)  
print('Coefficients:',regr.coef_) 
print ('Intercept:', regr.intercept_) 
predictedCO2=regr.predict([[3300,1300]]) 
print("predicted co2 for the correspin weight and vol, ",predictedCO2)


```
## Output:
![Screenshot 2025-04-30 114416](https://github.com/user-attachments/assets/a7d9efa5-6302-4d4f-924e-ccbaae202e6b)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
