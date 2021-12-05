# Instructions to use

1) Run `Dataset and its cleaning.ipynb`
2) It will generate 2 .csv files as output-
    * `cleaned_dataset_label_encoding.csv`
    * `cleaned_dataset_oneHot_encoding.csv`


# What does it cover?

1) This notebook takes 2 csv files - training and test as `inputs`.
2) It concatenates them generates single dataframe and does preprocessing on it.
    * Dropping extra columns
    * Dealing with errorenous values
    * Dealing with null values
    * Using encoding for categorical data
3) Generate 2 `output` csv files, one with one hot encoding and other with label encoding. 


Note- In the git hub repo, you may not find one or more output files uploaded. This is because they were more than the size that is allowed for an upload.
