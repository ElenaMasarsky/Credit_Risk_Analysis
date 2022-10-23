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
These are the results for all six machine learning models describing the balanced accuracy scores, the precision, and recall scores.

### Naive Random Oversampling
![pic](https://github.com/ElenaMasarsky/Credit_Risk_Analysis/blob/main/Resources/Naive%20Random%20Oversampling.png)  
* Balanced Accuracy: 0.6463970560994359  
* Precision:  High/Low risk = 0.01/1.00  
* Recall: High/Low risk = 0.71/0.58  

### SMOTE Oversampling
![pic](https://github.com/ElenaMasarsky/Credit_Risk_Analysis/blob/main/Resources/Naive%20Random%20Oversampling.png)  
* Balanced Accuracy: 0.6463970560994359 
* Precision:  High/Low risk = 0.01/1.00 
* Recall: High/Low risk = 0.71/0.58  


### Undersampling
![pic](https://github.com/ElenaMasarsky/Credit_Risk_Analysis/blob/main/Resources/Undersampling.png)  
* Balanced Accuracy: 0.5447339051023905
* Precision:  High/Low risk = 0.01/1.00 
* Recall: High/Low risk = 0.69/0.40  


### Combination (Over and Under) Sampling
![pic](https://github.com/ElenaMasarsky/Credit_Risk_Analysis/blob/main/Resources/Combination_Over_and_Under_Sampling.png)  
* Balanced Accuracy: 0.6480442302883235
* Precision:  High/Low risk = 0.01/1.00 
* Recall: High/Low risk = 0.72/0.57

### Easy Ensemble AdaBoost Classifier
![pic](https://github.com/ElenaMasarsky/Credit_Risk_Analysis/blob/main/Resources/Easy_Ensemble_AdaBoost_Classifier.png)  
* Balanced Accuracy: 0.9316600714093861
* Precision:  High/Low risk = 0.09/1.00   
* Recall: High/Low risk = 0.92/0.94


## Summary:  
When working with balanced accuracy, the highest compared accuracy closest to 1 is the best machine learning model. Balanced accuracy for all models exept Easy Ensemble AdaBoost Classifier gave us pretty low results.
All models showed low precision for high-risk loans and high for low-risk loans.
The best result of recall showed us the Easy Ensemble AdaBoost Classifier with the score for high and low risk 0.92/0.94 accordingly.  
The Easy Ensemble AdaBoost Classifier is the best machine learning model for this analysis.


