# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
Step1
Select any online compiler.

Step2
Type the required coding.

Step3
Import pandas.

Step4
Take a screenshot of the output and copy the program and the output in your git repository.

Step5
Push the output images and program in the git repository.
## Program:
```
'''
Developed by: SUROTHAAMAN R
Reference number: 212222103003
'''
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
![Uploading 284064973-c0c45e65-9e8d-4db6-9fa2-7d2f720184d3.png…]()


### Insert your output

<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
