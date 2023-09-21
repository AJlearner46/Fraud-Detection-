# Fraud-Detection

A data science project to predict whether a transaction is a fraud or not.

My solution to solve this problem will be the development of a data science project. This project will have a machine learning model which can predict whether a transaction is fraudulent or not.

### Step 01. 
Data Description: In this first section the data will be collected and studied. The missing values will be threated or removed. Finally, a initial data description will carried out to know the data. Therefore some calculations of descriptive statistics will be made.

### Step 02. 
Data visualization: In this section, diffrent type of relations of features are visulize by graphs and charts.

### Step 03. 
Exploratory Data Analysis: The exploratory data analysis section consists of univariate analysis, bivariate analysis and multivariate analysis to assist in understanding of the database.

### Step 04. 
Data Preparation: In this fifth section, the data will be prepared for machine learning modeling. Therefore, they will be transformed to improve the learning of the machine learning model, thus they can be encoded, oversampled, subsampled or rescaled.

## Step 05. 
Machine Learning Modeling: aims to train the machine learning algorithms and how they can predict the data. For validation the model is trained, validated and applied to cross validation to know the learning capacity of the model.

### Step 06. 
Hyparameter Fine Tuning: Firstly selected the best model to be applied in the project, it's important to make a fine tuning of the parameters to improve its scores. The same model performance methods apllied in the step 07 are used.

### Step 07. 
Conclusions: This is a conclusion stage which the generation capacity model is tested using unseen data. In addition, some business questions are answered to show the applicability of the model in the business context.


## Machine Learning Applied Model
Here's all cross validation results of the machine learning models with their default parameters. The cross validation method is important to show the capacity of the model to learn.

### LightGBM
![Screenshot 2023-09-21 223325](https://github.com/AJlearner46/Fraud-Detection-/assets/99804336/2841a932-f1a3-4601-aff7-9356d5d7f242)

### XGBoost
![Screenshot 2023-09-21 223311](https://github.com/AJlearner46/Fraud-Detection-/assets/99804336/31c12bb1-962a-4bea-ba5d-9a452618adc7)

## Machine Learning Performance
The chosen model was XGBoost and it was tuned to improve their parameters and scores. Below are final model with all hyper parameters.

#### Final Model

XGBClassifier  (  base_score=None,   booster='gbtree',   callbacks=None,  
                 colsample_bylevel=None,   colsample_bynode=None,  
                 colsample_bytree=None,   early_stopping_rounds=None,
                 enable_categorical=False,   eta=0.3,   eval_metric=None,  
                 feature_types=None,   gamma=None,   gpu_id=None,   grow_policy=None,  
                 importance_type=None,   interaction_constraints=None,  
                 learning_rate=None,   max_bin=None,   max_cat_threshold=None,  
                 max_cat_to_onehot=None,   max_delta_step=None,   max_depth=None,  
                 max_leaves=None,   min_child_weight=None,   missing=nan,  
                 monotone_constraints=None,   n_estimators=100,   n_jobs=None,  
                 num_parallel_tree=None,   predictor=None,   ...  )


              
Below there's a table with the capacity of the model to learn.
![Screenshot 2023-09-21 223534](https://github.com/AJlearner46/Fraud-Detection-/assets/99804336/e0fdaf88-6f38-41fb-966c-fd084944c12a)


It's possible to determinize the capacity of the model to generalize using unseen data. In other words, capcity of the model to classify new data as shown. 
![Screenshot 2023-09-21 223603](https://github.com/AJlearner46/Fraud-Detection-/assets/99804336/45b5fa2a-ee7e-42ad-8a2a-b6f1a470e9a6)


## Conclution

#### Precision : 0.97
 : Out of all the positive predicted, what percentage is truly positive.
 : fraud identified as fraud / total fraud prediction 

#### Recall : 0.873
 : Out of the total positive, what percentage are predicted positive.
 : fraud identified as fraud / actual total fraud

 
we need to protect user’s finances by trying to flag as many fraud transactions as possible while at the same time not mislabeling too many transactions so users can make transcation without the inconvenience of having transactions declined. 
