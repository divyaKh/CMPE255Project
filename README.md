# NETWORK ATTACK DETECTION

This repository is developed for group project for Team-8 in CMPE 255 class at San Jose State University Computer Engineering department - Fall 2021.

## INTRODUCTION

Cyber attacks are one of the biggest threads in this era of digital world. It is very important to combat the network attacks to establish a secure environment for all the users of a network. This project focuses on creating and testing Machine Learning Models over a large dataset of raw network packets to detect network attacks.

![image](https://www.incimages.com/uploaded_files/image/1920x1080/getty_483978146_116575.jpg)

## ABOUT DATASET

The dataset used, is created by Cyber Range Lab of UNSW Canberra. It is widely used and is named as UNSW-NB15 dataset. The raw network packets of the `UNSW-NB 15` dataset were created by the IXIA PerfectStorm tool. This data set has a hybrid of the real modern normal and the contemporary synthesized attack activities of the network traffic.

The UNSW-NB15  dataset can be found [here](https://research.unsw.edu.au/projects/unsw-nb15-dataset). 
We have used UNSW_NB15_training-set.csv and UNSW_NB15_testing-set.csv from the source and combined them to generate a single dataframe to work upon. For our work, the dataset contains `257,673 data records` with `49 features` as mentioned [here](https://cloudstor.aarnet.edu.au/plus/apps/onlyoffice/s/2DhnLGDdEECo4ys?fileId=206777051).

To know more about the dataset, read this [research](https://ieeexplore.ieee.org/abstract/document/7348942/authors#authors).

The dataset contains both categorical and numerical features with the count as given below-

|     Type       | Feature Count     | 
|----------------| ------------------|
|  Categorical   |       4            |
|  Numerical     |       45           |



## PROBLEM BEING INVESTIGATED

A network attack attempts to gain unauthorized access to the network. Using above mentioned dataset, we will detect that if any network attack is happening over the network. This dataset may have any of the following type of network attack:
* Fuzzers
* Analysis
* Backdoors
* Denial of Service
* Exploits
* Generic
* Reconnaissance
* Shellcode
* Worms 

The dataset is chosen because its competitor KDD-99 dataset has only four attack types DOS, R2L, U2R, and PROBE.

## PROJECT LIFECYCLE

1) Data Cleaning
  * Handle null values
  * Handle missing values
  * Drop unecessary columns
  * Encoding of Categorical Columns
  
2) Exploratory Data Analysis

3) Data Preprocessing
  * Min Max Scaling
  * Standard Scaling
  * Principal component Analysis
  * Correlation Analysis
  
4) Data Modeling
  * XGBoost
  * Gradient Boost
  * Decision Tree
  * Random Forest
  
5) Performance Metrics
  * Accuracy
  * F1 score
  * Receiver Operating Characteristic (ROC) curve
  * Area under the curve (AUC)
  * Confusion Matrix

## CONTRIBUTORS:

* [Divya Khandelwal](https://github.com/divyaKh)
* [Nancy Saxena](https://github.com/NancyS1)
* [Wen-Hao Tseng](https://github.com/Wenhao-Tseng)
* [Chintan Shah](https://github.com/chaks64)

## Instruction to run the code 

Stage 1: Go to the dataset run  https://github.com/divyaKh/CMPE255Project/blob/main/2.Data_Cleaning/Dataset_and_its_Cleaning.ipynb to get the https://github.com/divyaKh/CMPE255Project/blob/main/2.Data_Cleaning/cleaned_dataset_label_encoding.csv

Stage 2: Go to https://github.com/divyaKh/CMPE255Project/blob/main/3.EDA/Exploratory_Data_Analysis.ipynb and run it for the EDA

Stage 3: Go to https://github.com/divyaKh/CMPE255Project/blob/main/4.Preprocessing/pre_processing.ipynb and run it for MILETONE 3 preprocessing and 3 csvs.
We have changed a preprocessing a bit. We have taken on MINMAX scaler into consideration. 

Stage 4 : Go to https://github.com/divyaKh/CMPE255Project/tree/main/5.ML_Models/baseline run each notebook for each type of the models.This stage requires cleaned_dataset_label_encoding.csv,dataset_minmax.csv,dataset_minmax_corr.csv,dataset_pca.csv. These csv will be genrated at stage 1 and stage3. This is MILESTONE 3 implementation.

Each stage above will generate the csv, and fed to the next stage.

FOR Milestone 2 implementation -- > run https://github.com/divyaKh/CMPE255Project/blob/main/5.ML_Models/Final_notebook.ipynb. It has links to MILESTONE 3 implementations 
















