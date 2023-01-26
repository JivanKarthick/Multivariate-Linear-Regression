# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import pandas as pd.

### Step2
Read the csv file.

### Step3
Get the value of X and y variables.

### Step4
Create the linear regression model and fit

### Step5
Predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm3.

### Step6
Print the predicted output.

## Program:
```python
To write a python program to implement multivariate linear regression.
Developed by: Jivan Karthec.B.S
RegisterNumber: 22004763

import pandas as pd
from sklearn import linear_model
data=pd.read_csv("cars.csv")
x=data[['Weight','Volume']]
y=data['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print('coefficients: ',regr.coef_)
print('Intercet: ',regr.intercept_)
predictCO2=regr.predict([[3300,1300]])
print('Predicted CO2 for the corresponding Weight and Volume',predictCO2)
```
## Output:
![5](https://user-images.githubusercontent.com/121165867/214812375-c791e5ae-2444-4eaa-9497-45e6db4192f1.png)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
