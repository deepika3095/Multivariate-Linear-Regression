# DATE:
# EX-10 Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Start the program.
### Step2
Write a program to perform multivariate regression in anaconda navigator.
### Step3
Run the program.
### Step4
Print the output.
### Step5
End the program.
## Program:
```
#Program to find Univariate Linear Regression
#Developed by: DEEPIKA R
#Register number: 212223230038
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("cars.csv")
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print('Coefficients: ',regr.coef_)
print('Intercept:',regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print('Predicted CO2 for the corresponding weight and volume',predictedCO2)
```
## Output:
![image](https://github.com/user-attachments/assets/de834077-9b5c-4eeb-b441-f3ede3b000fc)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
