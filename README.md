# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import pandas

2.Import Decision tree classifier

3.Fit the data in the model

4.Find the accuracy score
## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: Shantharam M
RegisterNumber: 24900113
import pandas as pd
data=pd.read_csv("Salary.csv")
data.head()
data.info()
data.isnull().sum()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["Position"]=le.fit_transform(data["Position"])
data.head()
print(data.head())
x=data[["Position","Level"]]
print(x.head())
y=data["Salary"]
y.head()
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=2)
from sklearn.tree import DecisionTreeRegressor
dt=DecisionTreeRegressor()
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)
print(y_pred)
from sklearn import metrics
r2=metrics.r2_score(y_test,y_pred)
print(r2)
dt.predict([[5,6]])
*/
```
## Output:

![Screenshot 2024-11-28 192801](https://github.com/user-attachments/assets/85d85b8a-d8c1-45e9-bbed-8a4015b9b3a9)
![Screenshot 2024-11-28 192717](https://github.com/user-attachments/assets/3f1e9b5a-0759-4956-b42a-508ba948af9c)
![Screenshot 2024-11-28 192839](https://github.com/user-attachments/assets/fa881966-912f-4d2e-8e34-cf3703ded169)
![Screenshot 2024-11-28 193020](https://github.com/user-attachments/assets/635af721-68a6-4751-9f3f-e82e796dac12)


## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
