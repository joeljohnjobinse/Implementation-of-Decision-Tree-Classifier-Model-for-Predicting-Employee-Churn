# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Data Collection and Preprocessing
2. Model Training
3. Model Evaluation
4. Model Deployment and Monitoring

## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: Joel John Jobinse
RegisterNumber:  212223240062
import pandas as pd
data=pd.read_csv("C:/Users/admin/Downloads/Employee (1).csv")

data.head()

data.info()

data.isnull()

data.isnull().sum()

data['left'].value_counts()

from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()

data['salary']=le.fit_transform(data['salary'])
data.head()

x=data[['satisfaction_level','last_evaluation','number_project','average_montly_hours','time_spend_company','Work_accident','promotion_last_5years','salary']]
x.head()

y=data['left']
y.head()

from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=100)

from sklearn.tree import DecisionTreeClassifier
dt=DecisionTreeClassifier(criterion='entropy')
dt.fit(x_train,y_train)
y_predict=dt.predict(x_test)

from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_predict)
accuracy

dt.predict([[0.5,0.8,9,260,6,0,1,2]])
*/
```

## Output:
![image](https://github.com/joeljohnjobinse/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/138955488/8db9b260-4b19-410a-8252-58428f850d7e)

![image](https://github.com/joeljohnjobinse/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/138955488/1919e90f-b84c-4922-aa38-322d9e5b8c08)

![image](https://github.com/joeljohnjobinse/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/138955488/4d58de00-e475-40da-b39e-eec535114904)


## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
