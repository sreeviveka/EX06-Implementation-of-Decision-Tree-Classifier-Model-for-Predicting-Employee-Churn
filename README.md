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
3. Encode Categorical Variables. Use label encoding or one-hot encoding for categorical data (e.g., department, gender).
4. Split the Dataset: Divide the dataset into features (X) and target (y), then split into training and testing sets.
## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: Sreeviveka V.S 
RegisterNumber:  2305001031
*/
import pandas as pd
from sklearn.tree import Decision TreeClassifier, plot_tree from sklearn.preprocessing import LabelEncoder
import matplotlib.pyplot as plt
df-pd.read_csv("/content/Employee_EX6.csv")
data-df.copy()
data
le-LabelEncoder()
data['salary']=le.fit_transform(data['salary']) data
x=data.drop(['Departments', 'left'], axis-1) y=data['left']
clf-DecisionTreeClassifier()
clf,fit(x,y)
plt.figure(figsize=(80,80))
plot_tree(clf, feature_names=x.columns,class_names=['LEFT', 'NOT LEFT'], filled=True)
plt.show()
```

## Output:
![decision tree classifier model](sam.png)
![Screenshot 2024-10-17 101721](https://github.com/user-attachments/assets/c7cf0d84-6c12-45ca-99ca-56e43f1b7053)
![Screenshot 2024-10-17 101740](https://github.com/user-attachments/assets/defb1bc5-9b75-4297-a1a0-38c27e7865aa)
![Screenshot 2024-10-17 101749](https://github.com/user-attachments/assets/55091200-e00c-4d4e-af24-e43f9d6e78ab)
![WhatsApp Image 2024-10-17 at 10 19 10_aebea7c7](https://github.com/user-attachments/assets/dd9aa18c-4425-4114-bdc3-25a3d02a81cf)



## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
