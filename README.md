# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:

### Step1

Import the numpy module to use the built-in functions for calctions.
<br>

### Step2

Prepare the list from each linear equations and assign the np.array()
<br>

### Step3

Using the np.linalg.solve(),we can find the solutions.
<br>

### Step4

Execute the program.
<br>

### Step5

Successfully run the output.
<br>

## Program:
```
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("car.csv")
x=df[['weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print('Coefficients:',regr.coef_)
print('Intercept:',regr.intercept_)
predictedCO2=regr.predict(pd.DataFrame([[3300,1300]],columns=['Weight','Volume']))
print('Predicted CO2 for the corresponding weight and volume:',predictedCO2)
```

## Output:

### Insert your output

<img width="762" height="108" alt="Screenshot 2025-10-30 at 12 02 52 PM" src="https://github.com/user-attachments/assets/6affc572-8cda-47fe-972a-ce9a287c992b" />

<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
