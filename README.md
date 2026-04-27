# Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored

## AIM:
To write a program to predict the marks scored by a student using the simple linear regression model.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
```
1. Algorithm (Step-by-Step)
2.Import required libraries
3.Take input dataset (e.g., study hours vs marks scored)
4.Reshape data for model training
5.Split dataset into training and testing sets
6.Create a Linear Regression model
7.Train the model using training data
8.Predict marks using test data
9.Plot the regression line and data points
10.Display predicted results 
```
## Program:
```
/*
Program to implement the simple linear regression model for predicting the marks scored.
Developed by: Santhiya.G
RegisterNumber:  212225230248
# Program to implement simple linear regression model
# Developed by:
# Register Number:

import numpy as np
import matplotlib.pyplot as plt
from sklearn.linear_model import LinearRegression

# Sample dataset (Study Hours vs Marks)
X = np.array([1, 2, 3, 4, 5]).reshape(-1, 1)
Y = np.array([35, 50, 65, 70, 85])

# Create model
model = LinearRegression()

# Train model
model.fit(X, Y)

# Predict marks
Y_pred = model.predict(X)

# Display slope and intercept
print("Slope (m):", model.coef_[0])
print("Intercept (b):", model.intercept_)

# Plot graph
plt.scatter(X, Y, color='blue', label='Actual Data')
plt.plot(X, Y_pred, color='red', label='Regression Line')
plt.xlabel("Study Hours")
plt.ylabel("Marks Scored")
plt.title("Simple Linear Regression - Marks Prediction")
plt.legend()
plt.show()
*/
```

## Output:
<img width="914" height="622" alt="Screenshot 2026-04-27 105025" src="https://github.com/user-attachments/assets/0e2a25c0-084e-40bd-a3ea-2ae2915df028" />



## Result:
Thus the program to implement the simple linear regression model for predicting the marks scored is written and verified using python programming.
