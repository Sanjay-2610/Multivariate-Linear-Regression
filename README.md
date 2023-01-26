# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Importing panda as pd
### Step2
Importing linear_model from sklearn 

### Step3
Copying the contents from a csv file using panda 

### Step4
Saving the data to the list 
### Step5
Using LinearRegression() and fitting values from the csv file
### Step 6
Printing the co-efficient and the intercept from the LinearRegression
### Step 7
Predicting the value of C02 for the coresponding Weight and Volume and printing the value
## Program:
```py
#Program to find the multivariative linear regression
#Developed by: Sanjay Ragavendar M K
#RegisterNumber:22009286

import pandas as pd
from sklearn import linear_model
data=pd.read_csv('/content/cars (1).csv',)
x=data[['Weight','Volume']]
y=data['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print('Co efficient:',regr.coef_)
print('Intercept:',regr.intercept_)
predictedC02= regr.predict([[3300,1300]])
print('The predicted CO2 for the corresponding Weight and Volume is',predictedC02)

```
## Output:
![image](https://user-images.githubusercontent.com/91368803/214788744-678d48cf-c2ae-4d14-81ea-165c91d29aa1.png)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
