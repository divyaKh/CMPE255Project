# CMPE255Project
This repository is the group project for Team-8 in CMPE 255 class at SJSU CMPE department - Fall 2021
## Team members:
## Name - Github username

1)Nancy Saxena - NancyS1

2)Divya Khandelwal - divyaKh

3)Wen-Hao Tseng - Wenhao-Tseng

4)Chintan Shah - chaks64

# Project title: 

Predicting Network Attacks using UNSW-NB15 dataset. 

## What data you’ll use and where you’ll get it?

We will be using the UNSW-NB15 dataset. The raw network packets of the UNSW-NB 15 dataset was created by the IXIA PerfectStorm tool in the Cyber Range Lab of UNSW Canberra for generating a hybrid of real modern normal activities and synthetic contemporary attack behaviours.

The url to UNSW-NB15  dataset is:
https://research.unsw.edu.au/projects/unsw-nb15-dataset 
We will be using UNSW_NB15_training-set.csv and UNSW_NB15_testing-set.csv respectively. The number of records in the training set is 175,341 records and the testing set is 82,332 records.

There are 49 features which are mentioned :https://cloudstor.aarnet.edu.au/plus/apps/onlyoffice/s/2DhnLGDdEECo4ys?fileId=206777051


## Description of the problem we have solved or the question have investigated.

A network attack attempts to gain unauthorized access to the network. Using this dataset , we will predict the network attack that is happening over the network. This dataset has nine types of attacks, namely, Fuzzers, Analysis, Backdoors, DoS, Exploits, Generic, Reconnaissance, Shellcode and Worms unlike other dataset like KDD-99 dataset which has only four attack types DOS, R2L, U2R, and PROBE.

## Potential methods you have applied (these can change as you play with the data).

The datasets will be analysed and cleaned using a python script. For the model any classification algorithms can be used. However, we are considering decision trees. We will also consider other algorithm apart from Decision trees, like NN,KNN, Naive bayes etc. We are also considering :the different types of machine learning model  to build a hybrid learning mode.
![image](https://user-images.githubusercontent.com/79034901/138795426-a0a061d0-6a6f-442c-899f-490578660de8.png)

Source : https://www.researchgate.net/profile/Di-Wu-137/publication/330702257/figure/fig3/AS:720319446781952@1548748947667/Schematic-structure-of-hybrid-machine-learning-method.ppm


## Measuring success?

The success will be measured from the values of 
1. accuracy score of the model. 
2. confusion matrix which lets us know about the False Positives and False negatives.
3. F1 score
4. ROC curve 













