# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
Step 1:

Import the required libraries for data handling, model creation, and visualization.

Step 2:

Load the employee dataset and preprocess the data by converting categorical values into numerical format.

Step 3:

Split the dataset into training and testing sets and train the Decision Tree classifier model.

Step 4:

Test the model using the testing dataset, calculate the accuracy, and visualize the Decision Tree.

## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by:SARFARAZ I 
RegisterNumber: 212225230252
import pandas as pd
import matplotlib.pyplot as plt
from sklearn.model_selection import train_test_split
from sklearn.tree import DecisionTreeClassifier, plot_tree
from sklearn.metrics import accuracy_score
data = pd.read_csv("Employee.csv")
data = pd.get_dummies(data, drop_first=True)
X = data.iloc[:, :-1]
y = data.iloc[:, -1]
X_train, X_test, y_train, y_test = train_test_split(
    X, y, test_size=0.2, random_state=42
)
model = DecisionTreeClassifier(random_state=42)
model.fit(X_train, y_train)
y_pred = model.predict(X_test)
print("Accuracy:", accuracy_score(y_test, y_pred))
plt.figure(figsize=(20,10))
plot_tree(
    model,
    feature_names=X.columns,
    filled=True
)
plt.show()
*/
```

## Output:

<img width="1389" height="728" alt="image" src="https://github.com/user-attachments/assets/de067295-4ca8-4c5b-a712-2efaed9f1995" />


## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
