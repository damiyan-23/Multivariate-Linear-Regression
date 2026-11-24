# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
Step 1: Start the program.

Step 2: Import the required libraries such as NumPy and LinearRegression from Scikit-learn.

Step 3: Get the input data containing multiple independent variables and one dependent variable.

Step 4: Create a linear regression model using the LinearRegression() function and train the model using the given dataset.

Step 5: Predict the output for the given input values using the predict() function and display the result.

Step 6: Stop the program.

## Program:
```

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
<img width="1056" height="605" alt="Screenshot 2026-11-21 125528" src="https://github.com/user-attachments/assets/795524f0-0a7e-4e3e-9b84-e2facd989d47" />

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
