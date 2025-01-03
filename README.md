# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Input Data: 
Load the dataset using pd.read_csv("cars.csv").

### Step2
Prepare Features and Target:
  Assign X as the input features (weight, volume) and Y as the target variable (CO2).

### Step3
Create Model:
  Initialize a linear regression model using linear_model.LinearRegression().

### Step4
Train Model: 
  Fit the model to the data using regr.fit(X, Y).

### Step5
Output Results:
  Print the coefficients, intercept, and make predictions using regr.predict().
## Program:
```
# Developed by : ASTLE JOE A S
# Register No : 24004571

import pandas as pd
from sklearn import linear_model
data= pd.read_csv("cars.csv")

X=data[['Weight','Volume']]
Y=data['CO2']

regr=linear_model.LinearRegression()
regr.fit(X,Y)

print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)

predictCO2=regr.predict([[3300,1300]])
print("prediction CO2 for the corresponding weight and volume",predictCO2)





```
## Output:
![alt text](<WhatsApp Image 2024-12-27 at 09.22.52_98c14295.jpg>)

### Insert your output

<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
