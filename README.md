# Credit_Risk_Analysis

## Overview of the analysis: 
The purpose of this analysis is to create models that predict low_risk versus high_risk credit score applications by exploring different resampling methods for logistic regression.

## Results: 

 - Random Oversampling: Balanced_accuracy_score = .657, Precision = .99, Recall = .60

![](images/Roversampling.png)

 - SMOTE Oversampling: Balanced_accuracy_score = .662, Precision = .99, Recall = .69 

![](images/SMOTEoversampling.png)

 - Undersampling: Balanced_accuracy_score = .544, Precision = .99, Recall = .40

![](images/Undersampling.png)

 - Combination (Over and Under) Sampling - SMOTEENN: Balanced_accuracy_score = .688, Precision = .99, Recall = .57

![](images/SMOTEENN.png)

 - Balanced Random Forest Classifer: Balanced_accuracy_score = .789, Precision = .99, Recall = .87

![](images/brfc.png)

 - Easy Ensemble AdaBoost Classifer: Balanced_accuracy_score = .915, Precision = .99, Recall = .90

![](images/ensemble.png)

## Summary: 
Below is a comparison for the accuracy, precision, and recall for all 6 models. It is evident that the Easy Ensemble AdaBoost Classifer model did the best in each category, and therefore is highest recommended for this type of analysis.

### Comparing Balanced Accuracy Scores for the different models. 
Undersampling did the worst with about 54.4%. Both methods over oversampling and the method of combination sampling landed in the 60%-70% range, which is a little better. However, the Balanced Random Forest Classifer got 78.9%, while Easy Ensemble AdaBoost Classifer got the best with 91.5%

### Comparing Precision for the different models
All 6 models received an precision score of 99%. 

### Comparing Recall for the different models
The lowest recall score with 40% was undersampling. Combination did a little better with 57%. Random oversampling landed at 60%, while SMOTE oversampling had 69%. The best 2 methods for this category were the Balanced Random Forest Classifer with 87% and Easy Ensemble AdaBoost Classifer with 90%.

