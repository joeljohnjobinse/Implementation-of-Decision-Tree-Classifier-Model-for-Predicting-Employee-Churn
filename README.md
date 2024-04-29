# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
Step 1: Start

Step 2: Data Collection and Preprocessing

Step 3: Model Training

Step 4: Model Evaluation

Step 5: Model Deployment and Monitoring

Step 6: Stop

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
![image](https://github.com/joeljohnjobinse/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/138955488/fafe6420-9556-494e-baed-ca50341eaadd)

![image](https://github.com/joeljohnjobinse/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/138955488/e0930ad9-77bf-4f4b-a3f4-86f317dc5a63)

![image](https://github.com/joeljohnjobinse/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/138955488/6123ea2a-4421-4543-a85d-44add5c7b050)

![image](https://github.com/joeljohnjobinse/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/138955488/2ee9ff8b-fdf9-4ad9-9ee8-c2541d310ece)

![image](https://github.com/joeljohnjobinse/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/138955488/09e0b2f7-46f1-42b3-9a5e-1190df2f7a52)

![image](https://github.com/joeljohnjobinse/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/138955488/8d9c52f9-2270-4cec-b3e8-ad855795f314)

![image](https://github.com/joeljohnjobinse/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/138955488/555c77d3-29ad-4a32-ae78-bec8712f973d)

## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
