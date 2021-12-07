# Instruction to use :

Open the file and run all cells, and get the files.
1) The file contains some techniques to preprocess the files.
2) The functions have been designed for each steps.
3) Users can preprocess the file by calling the functions in the main function and get the preprocessed file by saving the data frame in "cleaned_dataset_label_encoding.csv"
From here : [https://github.com/divyaKh/CMPE255Project/blob/main/2.Data_Cleaning/cleaned_dataset_label_encoding.csv]

# PreProcessing Techniques used:

1) Feature Scaling
   * Minmax Scaling
   * Standard Scaling
3) Correlation Analysis
4) PCA


# Workflow

* `Input`: The script takes files that are output from Dataset/Dataset_and_its_Cleaning.ipynb. Find the input csv in the `input` folder.
* `Output`: It outputs 3 files. Find the output csv files in the `ouput` folder. (zipped due to size restrictions)
    * `dataset_minmax.csv`
    * `dataset_minmax_corr.csv`
    * `dataset_pca.csv`

Note: 
1) The main function can be changed according to the functions that are needed for the preprocessing the file. 
