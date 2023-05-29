# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
###Step1
import pandas as pd.

###Step2
Read the csv file.

###Step3
Get the value of X and y variables

###Step4
Create the linear regression model and fit.

###Step5
Predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm cube.
## Program:
```
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("/content/car.csv")
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print("predicted co@ for the corresponding weight and volume",predictedCO2)
```
## Output:
![WhatsApp Image 2023-05-29 at 14 26 06](https://github.com/lathishlathish/Multivariate-Linear-Regression/assets/120359170/ea8587d4-b31f-4129-b88d-4b6e3d153400)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
