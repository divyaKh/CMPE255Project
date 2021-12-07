# Instruction to use :

Open the file and run all cells, and get the files.
1) The file contains some techniques to preprocess the files.
2) The functions have been designed for each steps.
3) Users can preprocess the file by calling the functions in the main function and get the preprocessed file by saving the data frame in "train_preprocessed.csv" and "test_preprocessed.csv"

# PreProcessing Techniques used:

1) Feature Scaling
   * Minmax Scaling
   * Standard Scaling
3) Correlation Analysis
4) PCA


# Workflow

* `Input`: The script takes files that are output from Dataset/Dataset_and_its_Cleaning.ipynb.
* `Output`: It outputs 6 files, 3 with one hot ecoding and 3 with label encoding.
    * `data_minmax_labelenc.csv`
    * `dataset_minmax_corr_labelenc.csv`
    * `dataset_minmax_pca_labelenc.csv`

Note: 
1) The main function can be changed according to the functions that are needed for the preprocessing the file. 
2) Output csv files might not be uploaded because they exceeded the size limit of 100MB.
