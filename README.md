# EXPERIMENT NO: 10
# Implementation of Multivariate Linear Regression
#### NAME: AVINASH T
#### REG NO: 212223230026
#### DEPARTMENT: ARTIFICIAL INTELLIGENCE AND DATA SCIENCE
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
import pandas as pd.
### Step2
Read the csv file.
### Step3
Get the value of X and y variables
### Step4
Create the linear regression model and fit.
### Step5
Predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm cube.
## Program:
```
Developed by: AVINASG T
Reg.No: 212223230026
import pandas as pd
from sklearn import linear_model
df = pd.read_csv("carsemission.csv")
X = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X, y)
print('Coefficients:', regr.coef_)
print('Intercept:',regr.intercept_)
predictedCO2 = regr.predict([[3300, 1300]])
print('Predicted CO2 for the corresponding weight and volume',predictedCO2)
```
## Output:
![image](https://github.com/AVINASH05T/Multivariate-Linear-Regression/assets/151514286/947259b0-afb6-44cc-b790-120c5004a57c)
![image](https://github.com/AVINASH05T/Multivariate-Linear-Regression/assets/151514286/352b8963-216b-4e5f-ba61-80a069c622f4)
## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
