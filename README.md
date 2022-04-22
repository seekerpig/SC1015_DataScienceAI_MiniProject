# Telco Churn Prediction & Customer Clustering

## About
This is a mini project for SC1015 (Introduction to Data Science and Artificial Intelligence). In this project, we will be focusing on trying to predict whether a customer will churn or not based off on the context of a telecommunication dataset.

## Problem Definition
- Can we predict which customer will churn based on given customer variables?
- Can telco customers be clustered into different segments to better help the telco understand their customer segments and create targeted strategies?

## Problem Motivation
- Telco is one of the most competitive industry and in order to survive they have to maximise revenue.
- Research has shown that the highest ROI action to take is to increase customer retention
- Customer churn is a major problem for companies and it is important that we understand our customers and also predict whether if they will churn in advance to retain them. (Retention is better than acquisition)

## Files
- TelcoCus.csv - original telco file with no data preparation  
- cleanedTelco.csv - telco file with data preparation applied (this file is then used for classification and clustering notebook)
- 1_EDA_DataPrep.ipynb - First jupyter notebook to run - for data preparation, EDA and basic analysis
- 2_ClassificationModels.ipynb - Second Jupyter Notebook to Run - for Classification Modelling
- 3_ClusteringModel.ipynb - Third Jupyter Notebook to Run - For Clustering Modelling (Segmentation)


# Setup and Models
### Data Preparation
- Removed Null variables and useless columns.
- Created values for missing variables based off on calculation from existing variables
- Transforming Data types (e.g. int to object)
- One-Hot-Encoding

### Exploratory Data Analysis
- Explored the relationship between Churn and other variables in the dataset
- Analysed patterns between relationship and came up with some basic insights and analysis.
- KDEplots, boxplots, violin plots, pie charts and bar graphs are used.

### Classification (2 Attempts)
Attempt 1 uses standard train test split and default models with little to no tuning.  
Attempt 2 uses GridSearchCV to tune hyper parameters and also kfold cross validation to train and test data.
- Decision Tree
- Logistic Regression
- Random Forest
- Support Vector Classifier

### Clustering
- Kprototypes


## Team Members
Soh Zu Wei - Classification Models (with gridsearchcv, kfold & one-hot-encoding)  
Sanskkriti - Data Preparation and Exploratory Data Analysis  
Jue Lin - Clustering Models (Kprototypes)  

## Conclusion / Insights
- The four classification models provide similar accuracy results but based off on consistency, the two best classification model that the telco can use is Logistic Regression and Support Vector Classifier (median accuracy of 0.8)
- This implies that given a set of customer data, the telco will be able to predict whether the customer will churn or not with a good amount of accuracy and consistency, and thereby, this will help them to find out which customer are likely to churn. By finding out the customers that are likely to churn, the telco can actively work towards trying to retain these customers who are more likely to churn than those who are not.
- For clustering, based on the given data, we can effectively segment the customers into 4 types (low spenders, average spenders, high spenders with high average tenture and high spenders with low average tenure)
- Since each cluster have a distinct trait, This also means that telco can understand their different customer segments which helps in creating specific targeted marketing strategies for each of them (which is more effective than running a general fit all marketing strategy)






