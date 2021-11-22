---
title: Predicting Network Attack Using UNSW-NB15 Dataset
date: "November 2021"
author: 
- Divya Khandelwal
- Nancy Saxena 
- Chintan Shah
- Wen-Hao Tseng
- San José State University

header-includes: |
  \usepackage{booktabs}
  \usepackage{caption}
---

# Abstract

# Introduction
The occurrence of cyber security incidents have proliferated in recent years. Almost every year, one or two major information security incidents attract the attention of the world. Numerous studies have already been conducted in the field of cyber security utilizing data mining technologies. Using the UNSW-NB15 Dataset [@7348942], we will predict the network attack that is happening over the network. This dataset has nine types of attacks, namely, Fuzzers, Analysis, Backdoors, DoS, Exploits, Generic, Reconnaissance, Shellcode and Worms unlike other dataset like KDD-99 dataset which has only four attack types DOS, R2L, U2R, and PROBE. The attack distribution data of UNSW-NB15 is shown in Figure 1.  

![Figure 1](../distribution_pie_chart.png)

# Methods

# Comparisons

# 5 Data Analysis
### 5.1 Correlation Analysis – 
Correlation is a statistical analysis which is used for measuring and also describing the relation between different entities. In our data set we are using correlation feature selection for eliminating or dropping columns which have correlation factor more that 99%. Since the columns which are correlated with each other gives the same result, so pruning the correlated columns might reduce the complexity of the algorithm which will help in better analysis. After applying the correlation algorithm in our data set, there are 3 columns namely sloss, dloss and ct_ftp_cmd which are correlated to sbytes, dbytes, is_ftp_login respectively. Modeling of dataset was done using 4 different ML models i.e. XG Boost, Gradient Boost, Decision tree and Random Forest. We can see the comparison of modeling without correlation and with correlation. The accuracy of all the models hardly changed, for XG Boost accuracy increased from 94.9% to 95.1% while for decision tree it increased from 93.5% to 93.6% for others it remains unchanged. Hence, the correlation algorithm proved to be very efficient for us.

![image](https://user-images.githubusercontent.com/24936584/142936166-788579a3-0952-4b77-8a53-b97b87a74c6c.png)

![image](https://user-images.githubusercontent.com/24936584/142936128-14ee5b96-b926-4216-9554-610a855abe2f.png)

### Principal Component Analysis – 
Principal Component Analysis, or PCA, is a dimensionality-reduction method that is often used to reduce the dimensionality of large data sets, by transforming a large set of variables into a smaller one that still contains most of the information in the large set. But this dimensionality reduction technique may reduce the accuracy of any model at quite high rate, so this point needs to be considered while applying algorithm. We applied PCA algorithm with the variance of 99% on our data set. After applying number of rows were reduced from 42 to 29. But it cost the accuracy of every model.
Comparison can be inferred through following figures: 

-XG Boost: Without PCA accuracy was 93.4% but after applying PCA it reduced to 90.5%
![image](https://user-images.githubusercontent.com/24936584/142938935-70dfac8d-d46e-4579-b1fe-8f366ba9d9af.png)

-Gradient Boost: Accuracy without PCA was 94.8% which further reduced to 93%
![image](https://user-images.githubusercontent.com/24936584/142938889-34a60642-f0a3-4f4c-8f32-185c6e32be7b.png)

-Decision Tree: Accuracy without PCA was 94.9% which further reduced to 93.1%
![image](https://user-images.githubusercontent.com/24936584/142938843-38bb4166-b3a7-476d-988d-c600a18346e6.png)

-Random Forest: Accuracy without PCA was 96% which further reduced to 94.5%
![image](https://user-images.githubusercontent.com/24936584/142938794-cca3d728-969b-4c3b-bfa4-2fb1185e7d64.png)


# Conclusions


# References
