# Implementation-of-SVM-For-Spam-Mail-Detection

## AIM:
To write a program to implement the SVM For Spam Mail Detection.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import the required packages.
2.Import the dataset to operate on.
3.Split the dataset.
4.Predict the required output.

## Program:
```
/*
Program to implement the SVM For Spam Mail Detection..
Developed by: Daniel C
RegisterNumber: 212223240023


import chardet
file='/content/spam.csv'
with open(file,'rb') as rawdata:
  result = chardet.detect(rawdata.read(100000))
result


import pandas as pd
data=pd.read_csv('/content/spam.csv',encoding='Windows-1252')

data.head()

data.info()

data.isnull().sum()

x=data["v1"].values
y=data["v2"].values

from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=0)

from sklearn.feature_extraction.text import CountVectorizer
cv=CountVectorizer()

x_train=cv.fit_transform(x_train)
x_test=cv.transform(x_test)

from sklearn.svm import SVC
svc=SVC()
svc.fit(x_train,y_train)
y_pred=svc.predict(x_test)
y_pred

from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_pred)
accuracy
*/
```

## Output:
# Result output:
![image](https://github.com/Daniel-christal/Implementation-of-SVM-For-Spam-Mail-Detection/assets/145742847/b100b153-c540-4646-ab7e-dfc1555b6f3c)
# data.head():
![image](https://github.com/Daniel-christal/Implementation-of-SVM-For-Spam-Mail-Detection/assets/145742847/bd84e727-5c2a-4994-825b-14716145e3fd)
# data.info():
![image](https://github.com/Daniel-christal/Implementation-of-SVM-For-Spam-Mail-Detection/assets/145742847/ea594c8d-3130-4c5f-8491-d0939091422d)
# Y_prediction value:
![image](https://github.com/Daniel-christal/Implementation-of-SVM-For-Spam-Mail-Detection/assets/145742847/5897f7b2-5f81-4964-a42d-ac61564c59a7)
# Accuracy value:
![image](https://github.com/Daniel-christal/Implementation-of-SVM-For-Spam-Mail-Detection/assets/145742847/ebf9fbfa-30bd-43f2-a98a-25bc97daef14)


## Result:
Thus, the program to implement the SVM For Spam Mail Detection is written and verified using python programming.
