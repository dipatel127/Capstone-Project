# Capstone-Project
In this project, the application of machine learning to pharmaceutical dataset is considered. 
Datasets are given in CSV format in three different parts. 
First part of dataset contains all gene features and cell features along with other categorical parameters as reference to which features' value have been measured. 
The codes for Exploratory Data Analysis, Pincipal component analysis, and correlation analysis of this part of dataset is shown in notbook_train_features_R
Second part of dataset reflects labels for each instances. Since each instances has more than one class, this classification is turned out to be a multilabel classification
problem. The codes for Exploratory Data Analysis, and correlationa analysis of this part of dataset is shown in notbook_target_scored_R
Third part of dataset is actually a test dataset, to which a learned model from notbook_train_features_R will be applied.
EDA of train features and label datasets are performed in R.
classification model is performed in Python.
Binary Revelance is chosen as base model for classification. The code for this model is shown in notbook_Model_BR_Py
second order and higher order strategy of models will be also be considered for comaprison purpose....
