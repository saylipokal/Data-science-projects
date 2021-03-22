# Data-science-projects

## Employee-churn-classification

Objective: To predict employee attrition and to identify potential reasons for attrition.

Dataset: https://www.kaggle.com/pavansubhasht/ibm-hr-analytics-attrition-dataset/download

Approach:

The dataset is imbalanced in nature, directly implementing ML models may affect model precision.

1. Implemented under-sampling/over-sampling techniques to deal with the imbalance data. Compared the performance using precision and ROC curve.

2. Built a pipeline to implement all the steps in the process:
   -  Scaling/normalizing the data. 
   -  Implementing a sampling algorithm with a specific sampling rate.
   -  Implementing a classification method.

3. Compared the different sampling techniques and different classification algorithms to pick the best approach. 

Results:  

1. After exploring random undersampling, oversampling with SMOTE and a combination of under and over sampling, I found that all of them gave similar results. 
    I decided to implement random undersampling as it is the simplest and easiest method to explain. 

2. Currently, Random undersampling and Logitic regression gave the best result -- highest AUC score. In the future I will explore more methods. 


## Kaggle-Claims-Prediction 

Objective: To predict severity of insurance claims.

Dataset: https://www.kaggle.com/c/allstate-claims-severity/data

Approach:

1. Performed EDA and pre processing by one-hot encoding the categorical variables. 

2. Built ML models using Random Forest, XGBoost and LightGBM. 

3. Performed hyper-parameter tuning using randomized grid search and cross validation. 

4. Performed feature selection to see how the reduced models compare to the models built using all features. 

Results: 

1. LightGBM gave the best performance (lowest MAE) and took the least time to fit the models. 

2. The LightGBM model built using the top 50 important encoded features performed similar to the model using all 1000+ encoded features.   
