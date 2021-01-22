# Data-science-projects

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

2. The LightGBM model built using the top 50 important encoded features performed similar to the model using all encoded features.   
