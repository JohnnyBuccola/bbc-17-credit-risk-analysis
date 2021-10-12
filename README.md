# Challenge 17 - Credit Risk Analysis
## Overview
The purpose of this analysis is to select an algorithm that can best predict HIGH or LOW credit risk by training using historical credit information. This is done by using a number of resampling models and algorithms to find a configuration with the best fit based on their accuracy and precision scores.

## Results
After training each of 6 different algorithms, the balanced accuracy, precision, and recall scores were recorded for each algorithm.

- Logistic Regression using Random Oversampling
    - Balanced Accuracy Score: 0.634
    - Precision (HIGH RISK/LOW RISK): 0.01 / 1.0
    - Recall (HIGH RISK/LOW RISK): 0.61 / 0.66
- Logistic Regression using SMOTE Oversampling
    - Balanced Accuracy Score: 0.624
    - Precision (HIGH RISK/LOW RISK): 0.01 / 1.0
    - Recall (HIGH RISK/LOW RISK): 0.57 / 0.68
- Logistic Regression using Cluster Centroids Undersampling
    - Balanced Accuracy Score: 0.524
    - Precision (HIGH RISK/LOW RISK): 0.01 / 1.0
    - Recall (HIGH RISK/LOW RISK): 0.60 / 0.45
- Logistic Regression using SMOTEENN Sampling
    - Balanced Accuracy Score: 0.644
    - Precision (HIGH RISK/LOW RISK): 0.01 / 1.0
    - Recall (HIGH RISK/LOW RISK): 0.72 / 0.56
- Balanced Random Forest Classifier
    - Balanced Accuracy Score: 0.714
    - Precision (HIGH RISK/LOW RISK): 0.02 / 1.0
    - Recall (HIGH RISK/LOW RISK): 0.79 / 0.71
- Easy Ensemble AdaBoost Classifier
    - Balanced Accuracy Score: 0.750
    - Precision (HIGH RISK/LOW RISK): 0.02 / 1.0
    - Recall (HIGH RISK/LOW RISK): 0.79 / 0.71

## Summary

The results above show that there are some clear differences between the models, simply by looking at the balanced accuracy score of each.  On average, the random forest and ensemble classifiers performed somewhat better than logistic regressions. 

The best-performing algorithm all around is the __easy ensemble__, and is recommended for use due to its elevated sensitivity to high risk.  It should be noted that the algorithm is far from perfect, perhaps due to the highly imbalanced data set.