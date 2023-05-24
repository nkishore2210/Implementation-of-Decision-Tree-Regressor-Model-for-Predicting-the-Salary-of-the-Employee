# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import required packages and read the data file.

2.Use LabelEncoder to convert categorical data into numerical data.

3.Split data into testing data and training data. 

4.Apply Decision Tree Regressor. 

5.Calculate mean squared error and R2.

## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: N.Kishore
RegisterNumber: 212222240049  

import pandas as pd
data=pd.read_csv("/content/Salary.csv")
data.head()
data.head()
data.isnull()
data.isnull().sum()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["Position"]=le.fit_transform(data["Position"])
data.head()
x=data[["Position","Level"]]
y=data["Salary"]
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=2)
from sklearn.tree import DecisionTreeRegressor
dt=DecisionTreeRegressor()
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)
from sklearn import metrics
mse=metrics.mean_squared_error(y_test,y_pred)
mse
r2=metrics.r2_score(y_test,y_pred)
r2
dt.predict([[5,6]])
*/
```

## Output:

![image](https://github.com/nkishore2210/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/118707090/fde479e5-8007-4f24-8ab6-26e9676576ce)

![image](https://github.com/nkishore2210/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/118707090/5e88e334-6dd1-47dd-9dc9-f44ecae2208f)

![image](https://github.com/nkishore2210/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/118707090/362bd089-1a64-4d61-abd0-2bad8edfc4a3)

![image](https://github.com/nkishore2210/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/118707090/6a4e7642-fe74-475a-9abc-e2f08ce9fe92)

![image](https://github.com/nkishore2210/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/118707090/0ad7a9b6-4506-4428-8590-6c91f21c7a35)

![image](https://github.com/nkishore2210/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/118707090/106cd5f5-50fd-41d4-93bd-5a22674019fc)

![image](https://github.com/nkishore2210/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/118707090/2df39b4a-d4bc-4b67-b36f-4597cc8bda26)


## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
