# UNSW-NB15: Exploratory Data Analysis
For our work, the UNSW-NB15 dataset contains 257,673 data instances with 49 features. 
The total classes of this dataset are 10 classes: one is for a *normal* network data (93 000 instances) and nine classes of anomalous network data (attacks classes). 
The attacks involved were *backdoor* (2,329 instances), *analysis* (2,677 instances), *fuzzers* (24,246 instances), 
*shellcode* (1 511), *reconnaissance* (13,987 instances), *exploits* (44,525 instances), *DoS* (16,353 instances), 
worms (174 instances), and generic (58,871 instances). 
The data distribution data of UNSW-NB15 as in Figure 1.  
We perfomed 3 kinds of exploratory data analysis on the UNSW-NB15 dataset, 
namely countplot or barplot for all categorial or columns with small number of unique values, plot PDF for numerical features, and Correlation of the features and its heatmap.  
In this data set, there are total 9 attack categories of attack and normal is non-attack. The data is highly imbalanced and have lots of non-attack than attacks.
The most occured attack data categories are "*Reconnaissance*", "*Backdoor*", "*DoS*", "*Exploits*" and "*Analysis*". 
In the **protocol** category, most of the values are consists of udp and tcp. For attacks count of udp is lot higher. 
In **attack** data "dns" is present higher than any other values. There are few no of others and http also. 
In the **state** category we found the imbalce there are lots of int state for attacks.  
For numerical features, we plot PDF. For better visualization, we also used log scale. 
There are some results worth pointing out. **dload**: Destination bits per second, for attack data all the values are very close to 0. 
For normal data they are distributed all over, has values close to 0 and also very large values. **sbytes**: Source to destination bytes, Most of normal category values are close to 0. Attack categories has most of its values around 5 in log1p graph. 
The spread of values is wider in attack compared to normal.  
To Get correlation values for all the features, we plot heatmap of correaltion for better visualization. Most correlated features are: sbytes and sloss, sbytes and sloss, swin and dwin. 
These features are having very high correlation between them more 95%.
Although some features have high correlation between them, some of them is because they share same values, for instance, swin and dwin have correlation values is 99% between them. 
Even though these 2 columns are numerical but most of their values are only 0 and 255.

