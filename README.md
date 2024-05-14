# Implementation-of-K-Means-Clustering-for-Customer-Segmentation

## AIM:
To write a program to implement the K Means Clustering for Customer Segmentation.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. 
2. 
3. 
4. 

## Program:
```
/*
Program to implement the K Means Clustering for Customer Segmentation.
Developed by: P Mukteswara
RegisterNumber:  212223080039

import pandas as pd
import matplotlib.pyplot as plt
data = pd.read_csv("Mall_Customers.csv")

data.head()

data.isnull().sum()

from sklearn.cluster import KMeans
wcss=[]

for i in range(1,11):
 kmeans=KMeans(n_clusters=i,init="k-means++")
 kmeans.fit(data.iloc[:,3:])
 wcss.append(kmeans.inertia_)
plt.plot(range(1,11),wcss)
plt.xlabel("No.of clusters")
plt.ylabel("wcss")
plt.title("Elbow Method")

km=KMeans(n_clusters=5)
km.fit(data.iloc[:,3:])

y_pred=km.predict(data.iloc[:,3:])
y_pred


data["cluster"]=y_pred
df0=data[data["cluster"]==0]
df1=data[data["cluster"]==1]
df2=data[data["cluster"]==2]
df3=data[data["cluster"]==3]
df4=data[data["cluster"]==4]
plt.scatter(df0["Annual Income (k$)"],df0["Spending Score (1-100)"],c="red",label="cluster0")
plt.scatter(df1["Annual Income (k$)"],df1["Spending Score (1-100)"],c="black",label="cluster1")
plt.scatter(df2["Annual Income (k$)"],df2["Spending Score (1-100)"],c="blue",label="cluster2")
plt.scatter(df3["Annual Income (k$)"],df3["Spending Score (1-100)"],c="green",label="cluster3")
plt.scatter(df4["Annual Income (k$)"],df4["Spending Score (1-100)"],c="magenta",label="cluster4")
plt.legend()
plt.title("Customer Segments")
*/
```

## Output:
![8(1)](https://github.com/Mukteswara/Implementation-of-K-Means-Clustering-for-Customer-Segmentation/assets/162081121/0e75d667-efe6-4bce-8f1b-2e855251f553)
![8(2)](https://github.com/Mukteswara/Implementation-of-K-Means-Clustering-for-Customer-Segmentation/assets/162081121/ad421a82-3336-49b4-8e22-0818aa39a2fb)
![8(3)](https://github.com/Mukteswara/Implementation-of-K-Means-Clustering-for-Customer-Segmentation/assets/162081121/e03e4725-2e8e-4698-b55b-0e2217663aab)
![8(4)](https://github.com/Mukteswara/Implementation-of-K-Means-Clustering-for-Customer-Segmentation/assets/162081121/380d88ba-d67e-4a14-a657-3d03f27c983e)



## Result:
Thus the program to implement the K Means Clustering for Customer Segmentation is written and verified using python programming.
