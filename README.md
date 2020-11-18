# Capstone-Project
In this project, the application of machine learning to pharmaceutical dataset is considered. 
# DataSet
Datasets are given in CSV format in two different parts. Feature dataset and Label dataset can be found at [Kaggle](https://www.kaggle.com/c/lish-moa).
# Feature dataset
This dataset contains all gene features and cell features along with other categorical parameters as reference to which features' value have been measured. 
The codes for Exploratory Data Analysis, Pincipal component analysis, and correlation analysis of this part of dataset is shown in notbook_train_features_R
# Label dataset
This dataset reflects labels for each instances. Since each instances has more than one class, this classification is turned out to be a multilabel classification
problem. The codes for Exploratory Data Analysis, and correlationa analysis of this part of dataset is shown in notbook_target_scored_R
# EDA
EDA of feature and label datasets are performed in R. Since PCA did not reduce the dataset significantly, the entire dataset is used for model building.
# Data preprocessing
In feature dataset, all categorical features are converted to binary variables.
In the label dataset, sample IDs for which there was no activation of label has been removed entirly. 
Then both train dataset and label dataset are merged with common column which is sample id.
# Classification
Classification model is performed in Python.
Multioutput classification is chosen as base model for classification. The Random Forest is supplied as base classifier in this classification method.
For comparison purpose, two other models are developed : RakelD and Neural Network.
In all three models, repeated K fold cross validation method is used to create train and test dataset. Total 30 folds are created.
Accuracy, Log Loss, Hamming Loss, and Zero One Loss are used as evaluation metrics.
The mean and standard deviation of all results are taken into consideration as valid results.
