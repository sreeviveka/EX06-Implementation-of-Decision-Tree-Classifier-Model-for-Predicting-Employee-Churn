# EX 6 Implementation of Decision Tree Classifier Model for Predicting Employee Churn
## DATE:
## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Load the Dataset: Use pandas to load the dataset (CSV, Excel, etc.) into a DataFrame.
 2. Handle Missing Values: Identify and fill or drop missing values.
 3. Encode Categorical Variables: Use label encoding or one-hot encoding for categorical data
 (e.g., department, gender).
 4. Split the Dataset: Divide the dataset into features (X) and target (y), then split into training and
 testing sets

## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: Sreeviveka V.S
RegisterNumber:  2305001031
*/
 import pandas as pd
 from sklearn.tree import DecisionTreeClassifier, plot_tree
 from sklearn.preprocessing import LabelEncoder
 import matplotlib.pyplot as plt
 df=pd.read_csv("/content/Employee_EX6.csv")
 data=df.copy()
 data
 le=LabelEncoder()
 data['salary']=le.fit_transform(data['salary'])
 data
 x=data.drop(['Departments','left'],axis=1)
 y=data['left']
 clf=DecisionTreeClassifier()
 clf.fit(x,y)
 plt.figure(figsize=(80,80))
plot_tree(clf,feature_names=x.columns,class_names=['LEFT','NOT LEFT'],filled=True)
 plt.show()
```

## Output:
![decision tree classifier model](sam.png)
![WhatsApp Image 2024-10-17 at 14 02 17_9d7cc8c6](https://github.com/user-attachments/assets/90f04790-c3fe-4b7b-b236-d5240b6ae2d9)
![WhatsApp Image 2024-10-17 at 14 03 48_7e159de0](https://github.com/user-attachments/assets/92aa86bd-be7a-469b-9a18-a8f30a41e0df)
![WhatsApp Image 2024-10-17 at 14 04 21_16e23c9f](https://github.com/user-attachments/assets/76136fd1-f64e-4163-9b86-1d3528242489)
![WhatsApp Image 2024-10-17 at 14 04 52_ac2cd418](https://github.com/user-attachments/assets/30b62209-1d5c-407a-b65a-9a25a243ee22)


## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
