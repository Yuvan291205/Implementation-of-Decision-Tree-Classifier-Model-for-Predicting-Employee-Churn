# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import the required libraries.
2.Upload and read the dataset.
3.Check for any null values using the isnull() function.
4.From sklearn.tree import DecisionTreeClassifier and use criterion as entropy.
5.Find the accuracy of the model and predict the required values by importing the required module from sklearn.



## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: Yuvan M 
RegisterNumber:  212223240188

import pandas as pd
from sklearn.tree import DecisionTreeClassifier, plot_tree
data=pd.read_csv("Employee_EX6.csv")
data.head()
data.info()
data.isnull().sum()
data["left"].value_counts()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["salary"]=le.fit_transform(data["salary"])
data.head()
x=data[["satisfaction_level","last_evaluation","number_project","average_montly_hours","time_spend_company","Work_accident","promotion_last_5years","salary"]]
x.head()
y=data["left"]
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=100)
from sklearn.tree import DecisionTreeClassifier
dt=DecisionTreeClassifier(criterion="entropy")
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)
from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_pred)
accuracy
dt.predict([[0.5,0.8,9,260,6,0,1,2]])
plt.figure(figsize=(18,6))
plot_tree(dt,feature_names=x.columns,class_names=['salary','left'],filled=True)
plt.show()

*/
```

## Output:
### HEAD() AND INFO():
![image](https://github.com/Yuvan291205/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/138849170/a2f980fd-98b9-4f57-9e29-4e895b0a0fce)
### NULL AND COUNT:
![image](https://github.com/Yuvan291205/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/138849170/4816af31-efbd-490d-940f-5985d15eaff2)
![image](https://github.com/Yuvan291205/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/138849170/2109d3c7-846d-4752-b123-0b48263ae2d3)
### ACCURACY SCORE:
![image](https://github.com/Yuvan291205/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/138849170/e483f954-0e2c-4940-9e69-8cedd51d55d9)
### DECISION TREE CLASSIFIER MODEL:
![image](https://github.com/Yuvan291205/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/138849170/f317da5d-c1c7-40af-9309-7ec198bafd71)



## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
