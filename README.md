# Credit_Risk_Analysis

## Overview of the analysis:
Fast Lending, a peer lending services company wants to use machine leaning to predict credit risk. Management believes that this will provide a quicker and more reliable loan experience.
It also believes that machine learning will lead to a more accurate identification of good candidates for loans which will lead to lower default rates.
The company wants us to assist the lead Data Scientist in implementing this plan. 
In this project we build and evaluate several machine learning models or algorithms to predict credit risk. We use techniques such as resampling and boosting to make the most of our models and our data.
Once we've designed and implemented these algorithms, we evaluate their performance and see how well our models predict data. To acomplish our task, we use machine learning  algorithms,
statistics, and data processing techniques.
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, we need to employ different techniques to train and evaluate models with unbalanced classes.
That's why we use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.
Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, we oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm.
Then, we use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, we compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier,
to predict credit risk. Once we're done, we evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

## Results:
Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your results.
### Naive Random Oversampling

Balanced Accuracy: 0.6612700484668286
Precision: The precision is low for High-risk loans and is high for Low-risk loans.
Recall: High/Low risk = .66/.67
### SMOTE Oversampling

Balanced Accuracy: 0.6612700484668286
Precision: The precision is low for High-risk loans and is high for Low-risk loans.
Recall: High/Low risk = .66/.67

### Undersampling

Balanced Accuracy: 0.6612700484668286
Precision: The precision is low for High-risk loans and is high for Low-risk loans.
Recall: High/Low risk = .66/.67

### Combination Under-Over Sampling

Balanced Accuracy: 0.6612700484668286
Precision: The precision is low for High-risk loans and is high for Low-risk loans.
Recall: High/Low risk = .66/.67

### Easy Ensemble AdaBoost Classifier

Balanced Accuracy: 0.6612700484668286
Precision: The precision is low for High-risk loans and is high for Low-risk loans.
Recall: High/Low risk = .66/.67

Summary:
Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.

When working with balanced accuracy, the highest compared accuracy between 0 and 1 and is closest to 1 is the best machine learning model. For the credit card data set, the Easy Ensemble AdaBoost Classifier is the best model to choose with its .93 balanced accuracy.
The other models were below .80 balanced accuracy. The precision for all models were similar and within an appropriate range. The recall score also needs to fall within 0 and 1, with numbers closer to 1 being the better model.
The Easy Ensemble AdaBoost Classifier had the highest recall score, making it the final best machine learning model to choose for further credit card analysis.

When working with balanced accuracy, the highest compared accuracy closest to 1 is the best machine learning model. For the credit card data set, the Easy Ensemble AdaBoost Classifier is the best model to choose with its .93 balanced accuracy.
The other models were below .78 balanced accuracy. For the recall score, the numbers closer to 1 would be the better model. The Easy Ensemble AdaBoost Classifier had the highest recall score (0.91/0.94).
The Easy Ensemble AdaBoost Classifier is the best machine learning model according to my analysis.

All models with resampling data showed pretty low accuracy score, but in the imbalanced classification report we can see that all models predicted low_risk better and a presision rate is 1 in all reports. 
The SMOTE model has better F1 score which is 0.81 and could be a possible choise for choosing a model for predictions in the certain circumstances.
 The models with Ensemble Learners showed better results, especially EasyEnsembleClassifier showed accuracy score as 0,93 which is the highest from all the models, Also, its presision and F1 scores looks pretty high.
 So from all the presented models in this challenge the EasyEnsembleClassifier is recomendation to use.