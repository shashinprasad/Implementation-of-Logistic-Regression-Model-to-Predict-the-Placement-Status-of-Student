# Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student

## AIM:
To write a program to implement the the Logistic Regression Model to Predict the Placement Status of Student.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import pandas for data manipulation and sklearn for machine learning operations.
2. Load data from a CSV file using pandas, then preprocess it by removing unnecessary columns and handling missing values if any. 
3. Divide the preprocessed data into training and testing sets.
4. Train a machine learning model, such as logistic regression (lr), on the training data.

## Program:

/*
Program to implement the the Logistic Regression Model to Predict the Placement Status of Student.

Developed by:Shashin prasad S

RegisterNumber: 212222230144
*/
```
import pandas as pd
data = pd.read_csv("/content/Placement_Data.csv")
data.head()
data1=data.copy()
data1=data1.drop(["sl_no","salary"],axis=1)
data1.head()
data1.isnull().sum()
data1.duplicated().sum()
x=data1.iloc[:,:-1]
x
y=data1["status"]
y
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=0)
from sklearn.metrics import accuracy_score
accuracy = accuracy_score(y_test,y_pred)
accuracy
from sklearn.metrics import confusion_matrix
confusion = (y_test,y_pred)
confusion
from sklearn.metrics import classification_report
classification_report1 = classification_report(y_test,y_pred)
print(classification_report1)
lr.predict([[1,80,1,90,1,1,90,1,0,85,1,85]])
```

## Output:
![314367688-32d647e7-f70f-4fba-a8e6-8b16201c475c](https://github.com/AdhithiyanK/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/121029258/ee5ffe95-5d8b-45fe-b47a-0fabee03005a)

![314367740-2f62e9d3-7684-44e8-a969-4eddcbe808d3](https://github.com/AdhithiyanK/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/121029258/030f1075-9010-432c-b281-e5a179652059)

![314367779-e2633c37-45a7-4b28-83f1-77ab15765e1e](https://github.com/AdhithiyanK/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/121029258/9c94bb85-eb03-418f-8ab2-86063503c7ed)

![314367834-38361f24-94ec-42de-aa6e-14d67d3304ad](https://github.com/AdhithiyanK/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/121029258/93a1be74-719c-4c80-9c60-3d32a91b7ff5)

![314367896-89fee1bc-aabc-4868-b12e-7019d1f117da](https://github.com/AdhithiyanK/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/121029258/286966b0-8d74-486d-aeb5-29dc8dcc71fd)

![314368328-41b02477-baa5-487c-9c06-264d895097da](https://github.com/AdhithiyanK/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/121029258/6aa18ca6-f888-4065-9f1a-55a598e522b4)

![314368412-637b03a9-3ad4-4390-8dc4-7ccd82119d9f](https://github.com/AdhithiyanK/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/121029258/7e4c3ee8-32a7-4547-b92f-97f0c6f6fd10)

![314368575-42e96505-13fb-457d-9d81-d76d1486d5a9](https://github.com/AdhithiyanK/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/121029258/9367a2e9-890a-4468-ba31-9de8e37c504d)


![314368600-5e57cad1-6a4d-409b-a63d-a71657d5d2f2](https://github.com/AdhithiyanK/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/121029258/358078e2-81b1-4e81-96bf-ae692416af9e)

![314368653-75502ec7-8b17-40dd-a575-db8c6d0e6e97](https://github.com/AdhithiyanK/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/121029258/ff912a32-7469-4447-9ce4-0da6953607b4)


![314368690-9baf5590-6c48-4a0f-8162-111459350534](https://github.com/AdhithiyanK/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/121029258/379bd283-68fb-47b2-a7e7-43fb3c1731a6)

## Result:
Thus the program to implement the the Logistic Regression Model to Predict the Placement Status of Student is written and verified using python programming.
