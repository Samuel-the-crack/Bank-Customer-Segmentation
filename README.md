# Bank-Customer-Segmentation
Performing a clustering model for Bank Customer Dataset using K-Means clustering 


<p align="center">
<img src = "https://github.com/Samuel-the-crack/Bank-Customer-Segmentation/blob/main/Picture/Increasing-Customer-Loyalty-in-the-Banking-Industry.png" width = '800'>

## A. Background 
To increase the flow of money in this bank, the digital marketer team want to know what customer segment that have the highest balance percentage. This process is important to know what kind of services that suits best for this kind of customer. In this model I'm using [K-Means](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html) Clustering as the main algorithm. 

**Requirements : numpy, pandas, matplotlib, seaborn, sklearn, yellowbrick**
  
## B. Overview 
In this model I'm using three-level clustering. First clustering was separate the balane's outliers and non outliers, this analysis was helped with boxplot diagram.
<p align='center'>
<img src = "https://github.com/Samuel-the-crack/Bank-Customer-Segmentation/blob/main/Picture/boxplot.JPG" width = '400'>

from the boxplot above I separate the data into to cluster, avg_balance and high_balance. 

The second clustering was the use of K-Means clustering algorithm based on "balance", "age", "duration" for each cluster in first clustering, and this is the result of the second clustering.
<p align='center'>
<img src = "https://github.com/Samuel-the-crack/Bank-Customer-Segmentation/blob/main/Picture/Cluster.JPG" width = '700'>
 
After knowing the main cluster, the last clustering level was clustering it again based on it's 'job', 'marital', and 'education'. The result of the segment that has the highest balance can bee seen in the table below (high balanced data).
<p align='center'>
<img src = 'https://github.com/Samuel-the-crack/Bank-Customer-Segmentation/blob/main/Picture/Groupby%20high%20balance.JPG' width = '600'>
  
And for the average balance data can be seen also at the table below.
<p align='center'>
<img src = 'https://github.com/Samuel-the-crack/Bank-Customer-Segmentation/blob/main/Picture/groupby%20avg%20balance.JPG' width = '600'>

from two table above we can conclude that both of them were in their early thirty, single, have tertiary level education, and work in management field. with that information digital marketing team can calculate the best service for them. 
  
**For complete code you can se it [here](https://github.com/Samuel-the-crack/Bank-Customer-Segmentation/blob/main/FinalProject_Samuel.ipynb)**
