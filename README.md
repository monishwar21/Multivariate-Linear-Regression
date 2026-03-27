# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
##NAME: MONISHWAR K
##REGISTER NUMBER:212225230188
### Step1
<br>
import pandas as pd
### Step2
<br>
Read the csv file.
### Step3
<br>
Get the value of X and y variables
### Step4
<br>
Create the linear regression model and fit.
### Step5
<br>

Predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm cube.
## Program:
```

#Ex10- Multivariate Linear Regression

import pandas as pd
from sklearn import linear_model
df = pd.read_csv("carsemission.csv")
X = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X, y)
print('Coefficients:', regr.coef_)
print('Intercept:', regr.intercept_)
input_data = pd.DataFrame({'Weight': [3300], 'Volume': [1300]})
predictedCO2 = regr.predict(input_data)
print('Predicted CO2 for the corresponding weight and volume:', predictedCO2)






```
## Output:
<img width="1595" height="598" alt="image" src="https://github.com/user-attachments/assets/8a25c30d-ca41-4c65-bcea-5da1b511f4aa" />


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
