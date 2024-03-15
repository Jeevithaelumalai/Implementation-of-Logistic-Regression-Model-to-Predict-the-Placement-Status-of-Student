# Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student

## AIM:
To write a program to implement the the Logistic Regression Model to Predict the Placement Status of Student.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import the required packages and print the present data
2. Print the placement data and salary data.
3. Find the null and duplicate values.
4. Using logistic regression find the predicted values of accuracy , confusion matrices 

## Program:
```
/*
Program to implement the the Logistic Regression Model to Predict the Placement Status of Student.
Developed by: Jeevitha E
RegisterNumber: 212222230054 
*/
```
```
import pandas as pd
data =pd.read_csv('Placement_Data.csv')
data.head()
data1=data.copy()
data1= data1.drop(["sl_no","salary"],axis = 1)
data1.head
data1.isnull().sum()
data1.duplicated().sum()
from sklearn.preprocessing import LabelEncoder
le = LabelEncoder()
data1["gender"] = le.fit_transform(data1["gender"])
data1["ssc_b"] = le.fit_transform(data1["ssc_b"])
data1["hsc_b"] = le.fit_transform(data1["hsc_b"])
data1["hsc_s"] = le.fit_transform(data1["hsc_s"])
data1["degree_t"] = le.fit_transform(data1["degree_t"])
data1["workex"] = le.fit_transform(data1["workex"])
data1["specialisation"] = le.fit_transform(data1["specialisation"])
data1["status"] = le.fit_transform(data1["status"])
data1
x = data1.iloc[:,:-1]
x
y = data1["status"]
y
```

## Output:
![image](https://github.com/Jeevithaelumalai/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/118708245/addba76c-e254-4db6-897d-bdb95c7c42bd)
![image](https://github.com/Jeevithaelumalai/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/118708245/72190a7e-8937-4a4a-82b7-0e6ec0b4cd46)
![image](https://github.com/Jeevithaelumalai/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/118708245/42278e84-c3ab-4d16-a54b-046a2590023c)
![image](https://github.com/Jeevithaelumalai/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/118708245/cc98ed7a-f842-46d9-89c0-4b735855c1c4)
![image](https://github.com/Jeevithaelumalai/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/118708245/b1a8c8fb-f704-4b41-b0c2-19897524b3d4)
![image](https://github.com/Jeevithaelumalai/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/118708245/8314d6b6-18bc-43ed-9849-75e13db7344c)
![image](https://github.com/Jeevithaelumalai/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/118708245/bebeb524-c1ad-41df-ad0d-19fbf0487d6d)
![image](https://github.com/Jeevithaelumalai/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/118708245/e4d6e393-9cd4-4093-89b4-5ec22ecea9ce)
![image](https://github.com/Jeevithaelumalai/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/118708245/7ec88af2-77ce-4dba-8a09-85598f94259a)


## Result:
Thus the program to implement the the Logistic Regression Model to Predict the Placement Status of Student is written and verified using python programming.
