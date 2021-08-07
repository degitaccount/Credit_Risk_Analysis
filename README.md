# Credit_Risk_Analysis

### Analysis Overview
This analysis leverages machine learning Resampling Models, SMOTEEN Algorithm and Ensemble Classifiers to predict credit risk.

### Results
*Naive Random Oversampling*

* Balanced Accuracy Score = [(sensitivity: 68% + specificity: 59%) / 2] = 64%
* High-risk precision is 1% and the low F1 score of 2% highlights that there is an imbalance between the sensitivity (or recall) and precision
* Low-risk precision is 100% and the sensitivity score suggests the model can predict this risk accurately about 68% of the time


![NaïveRandomOversampling.PNG]( https://github.com/degitaccount/Credit_Risk_Analysis/blob/main/NaiveRandomOversampling.PNG)


*SMOTE Oversampling*

* Balanced Accuracy Score = [(sensitivity: 62% + specificity: 64%) / 2] = 63%
* High-risk precision is 1% and the low F1 score of 2% highlights that there is an imbalance between the sensitivity (or recall) and precision
* Low-risk precision is 100% and the sensitivity score suggests the model can predict this risk accurately about 62% of the time
* The overall results are very similar to the Naive Random Oversampling model.


![SMOTEOversampling.PNG]( https://github.com/degitaccount/Credit_Risk_Analysis/blob/main/SMOTEOversampling.PNG)

 
*Undersampling*

* Balanced Accuracy Score = [(sensitivity: 45% + specificity: 61%) / 2] = 53%
* High-risk precision is 1% and the low F1 score of 1% highlights that there is an imbalance between the sensitivity (or recall) and precision
* Low-risk precision is 100% and the sensitivity score suggests the model can predict this risk accurately about 45% of the time


![UnderSampling.PNG]( https://github.com/degitaccount/Credit_Risk_Analysis/blob/main/UnderSampling.PNG)
 

*Combination (Over and Under) Sampling*

* Balanced Accuracy Score = [(sensitivity: 57% + specificity: 67%) / 2] = 62%
* High-risk precision is 1% and the low F1 score of 2% highlights that there is an imbalance between the sensitivity (or recall) and precision
* Low-risk precision is 100% and the sensitivity score suggests the model can predict this risk accurately about 57% of the time


![ CombinationOverUnderSampling.PNG]( https://github.com/degitaccount/Credit_Risk_Analysis/blob/main/CombinationOverUnderSampling.PNG)
 

*Balanced Random Forest Classifier*

* Balanced Accuracy Score = [(sensitivity: 91% + specificity: 67%) / 2] = 79%
* High-risk precision is 4% and the low F1 score of 7% highlights that there is an imbalance between the sensitivity (or recall) and precision, although the F1 score slightly better than shown in the previous models
* Low-risk precision is 100% and the sensitivity score suggests the model can predict this risk accurately about 91% of the time


![EnsembleRandomeForrest.PNG]( https://github.com/degitaccount/Credit_Risk_Analysis/blob/main/EnsembleRandomeForrest.PNG)
 

*Easy Ensemble AdaBoost Classifier*

* Balanced Accuracy Score = [(sensitivity: 94% + specificity: 91%) / 2] = 93%
* High-risk precision is 7% and the low F1 score of 14% highlights that there is an imbalance between the sensitivity (or recall) and precision, however the F1 score is the highest among all of the models
* Low-risk precision is 100% and the sensitivity score suggests the model can predict this risk accurately about 94% of the time


![EnsembleAdaBoost.PNG]( https://github.com/degitaccount/Credit_Risk_Analysis/blob/main/EnsembleAdaBoost.PNG)
 

### Summary
All of the models tested demonstrated a high degree of accuracy in predicting low risk, however they do not perform nearly as well in predicting high risk.  The Easy Ensemble AdaBoost Classifier model performed best at predicting risk in both categories.  However, the model is still very weak at predicting high risk so for this reason I would not recommend using any of these models for assessing credit risk.  

