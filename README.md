# Implementation-of-Linear-Regression-Using-Gradient-Descent

## AIM:
To write a program to predict the profit of a city using the linear regression model with gradient descent.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. **Import Libraries**: Load necessary libraries for data handling, metrics, and visualization.

2. **Load Data**: Read the dataset using `pd.read_csv()` and display basic information.

3. **Initialize Parameters**: Set initial values for slope (m), intercept (c), learning rate, and epochs.

4. **Gradient Descent**: Perform iterations to update `m` and `c` using gradient descent.

5. **Plot Error**: Visualize the error over iterations to monitor convergence of the model.

## Program:
```
/*
Program to implement the linear regression using gradient descent.
Developed by: GEDIPUDI DARSHANI
RegisterNumber: 212223230062 
*/
```
```
import pandas as pd
import numpy as np
df=pd.read_csv("50_Startups.csv")
df.head()
```
## Output:
![image](https://github.com/user-attachments/assets/8f90c7d5-426e-4064-b153-c09e9124df83)
```
df.tail()
```
## Output:
![image](https://github.com/user-attachments/assets/1abb8d2d-8210-4075-89a0-f15962867308)
```
df.info()
```
## Output:
![image](https://github.com/user-attachments/assets/4428ec26-0d62-4d45-9dd9-7d5b71366f42)
```
x=(df.iloc[1:,:-2].values)
y=(df.iloc[1:,-1].values).reshape(-1,1)
print(y)
```
## Output:
![image](https://github.com/user-attachments/assets/0f446bef-ffbd-4fa4-b0e7-e20280e3f52a)
```
print(x)
```
## Output:
![image](https://github.com/user-attachments/assets/56423a39-54c9-4e20-aad1-cec73c06ffe7)
```
from sklearn.preprocessing import StandardScaler
scaler=StandardScaler()
x1_scaled=scaler.fit_transform(x)
y1_scaled=scaler.fit_transform(y)
print(x1_scaled)
print(y1_scaled)
```
## Output:
![image](https://github.com/user-attachments/assets/cf5029ad-12a4-4c76-b08d-00eedfaa7382)
![image](https://github.com/user-attachments/assets/cdece828-f185-43e8-8c69-7ccfc65d167d)
```
def multivariate_linear_regression (x1,y,learning_rate=0.01,num_iterations=100):
  theta=multivariate_linear_regression(x1_scaled,y1_scaled)
x=np.c_[np.ones(len(x1_scaled)),x1_scaled]
num_iterations=100
```
## Result:
Thus the program to implement the linear regression using gradient descent is written and verified using python programming.
