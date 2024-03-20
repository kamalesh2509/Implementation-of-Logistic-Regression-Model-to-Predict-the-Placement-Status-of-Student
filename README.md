![314367688-32d647e7-f70f-4fba-a8e6-8b16201c475c](https://github.com/kamalesh2509/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/120444689/abf888b7-def6-430f-ad1f-bf775b1d55f9)# Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student

## AIM:
To write a program to implement the the Logistic Regression Model to Predict the Placement Status of Student.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import pandas for data manipulation and sklearn for machine learning operations.
   
2. Load data from a CSV file using pandas

3.  then preprocess it by removing unnecessary columns and handling missing values if any.
   
4. Train a machine learning model, such as logistic regression (lr), on the training 
   data.
   
5.Calculate accuracy, generate confusion matrix, and produce a classification report to 
  assess model performance.
  
6. Utilize the trained model to make predictions on new data points, ensuring it's 
   fitted on training data before predicting on the test set.

## Program:
```
/*
Program to implement the the Logistic Regression Model to Predict the Placement Status of Student.
Developed by: E Kamalesh
RegisterNumber:  212222100019
*/
```
```import pandas as pd
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
![314367688-32d647e7-f70f-4fba-a8e6-8b16201c475c](https://github.com/kamalesh2509/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/120444689/f5a1dc40-1625-4b34-9fee-0bb4daf6ce9a)

![314367740-2f62e9d3-7684-44e8-a969-4eddcbe808d3](https://github.com/kamalesh2509/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/120444689/04756a25-6ac5-4e42-a1ab-a709e627a4cd)
![314367779-e2633c37-45a7-4b28-83f1-77ab15765e1e](https://github.com/kamalesh2509/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/120444689/ca178c90-2866-4211-94dc-cc4fa56b41f1)
![314367834-38361f24-94ec-42de-aa6e-14d67d3304ad](https://github.com/kamalesh2509/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/120444689/2fa472f6-ff65-4d9a-a16e-8f1123563f8c)
![314367834-38361f24-94ec-42de-aa6e-14d67d3304ad](https://github.com/kamalesh2509/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/120444689/89a093a2-4f6a-4ec4-9b2e-977321793f0a)
![314368328-41b02477-baa5-487c-9c06-264d895097da](https://github.com/kamalesh2509/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/120444689/5c9afade-522d-4012-af30-840e75b7ea0f)

![314368412-637b03a9-3ad4-4390-8dc4-7ccd82119d9f](https://github.com/kamalesh2509/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/120444689/bf592870-0fe4-45bd-9d01-dc6c9ebe34f7)
![314368575-42e96505-13fb-457d-9d81-d76d1486d5a9](https://github.com/kamalesh2509/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/120444689/bbebbfe7-9b3e-406c-9001-0f33638fb800)
![314368600-5e57cad1-6a4d-409b-a63d-a71657d5d2f2](https://github.com/kamalesh2509/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/120444689/802af8d3-be5e-4df0-a587-28a79594d441)

![314368653-75502ec7-8b17-40dd-a575-db8c6d0e6e97](https://github.com/kamalesh2509/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/120444689/7dbbd1a5-bc02-471c-9c8e-16cda477a83f)
![314368653-75502ec7-8b17-40dd-a575-db8c6d0e6e97](https://github.com/kamalesh2509/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/120444689/489f419b-d701-4309-9e40-27223eadab05)

## Result:
Thus the program to implement the the Logistic Regression Model to Predict the Placement Status of Student is written and verified using python programming.
