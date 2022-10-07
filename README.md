# Credit_Risk_Analysis

## Overview of the Analysis
The purpose of this analysis was to test a machine learning program in its ability to accurately determine credit card risk using RandomOverSampler and SMOTE algorithims for oversampling, and the ClusterCentroids algorithim for undersmapling. The model was also testied using the BalancedRandomForestClassifier and the EasyEnsembleClassifier to predict credit credit risk. The various methods of using the data to help the program learn were evaluated at the end to determine which was the most effective.

## Results

### Naive Random Oversampling
![Naive](https://user-images.githubusercontent.com/107013312/194456273-203d23a2-a630-442c-b4ca-04f9cf0fd6b7.png)

Balanced Accuracy = .637
High Risk Percision = .01
Low Risk Percision = 1.00

### SMOTE Oversampling
![SMOTE](https://user-images.githubusercontent.com/107013312/194456288-555a45b7-c6f1-4d95-8404-7fb52ed4f41f.png)

Balanced Accuracy = .630
High Risk Percision = .01
Low Risk Percision = 1.00

### Cluster Centroids Undersmapling
![Undersampling](https://user-images.githubusercontent.com/107013312/194456303-90ab3238-bf7a-4bcd-a429-a83052551ea1.png)

Balanced Accuracy = .522
High Risk Percision = .01
Low Risk Percision = 1.00

### Combination (Over and Under) Sampling
![Combination](https://user-images.githubusercontent.com/107013312/194456328-6ebb1bb2-eaa1-47c2-83f7-b404547eb638.png)

Balanced Accuracy = .653
High Risk Percision = .01
Low Risk Percision = 1.00

### Balanced Random Forest Classifier
![Balanced_Random_Forest_Classifier](https://user-images.githubusercontent.com/107013312/194456344-b4c27b95-b33d-456e-8b84-cad8219a70c5.png)

Balanced Accuracy = .789 
High Risk Percision = .03
Low Risk Percision = 1.00

### Easy Ensemble AdaBoost Classifier
![Easy_Ensemble](https://user-images.githubusercontent.com/107013312/194456351-5eef6aa3-10cf-4f12-9efe-8bed9e0c9ba9.png)

Balanced Accuracy = .932
High Risk Percision = .09
Low Risk Percision = 1.00

## Summary

### Recommendation




Undersampling was by far the least effective method. The two oversampling methods as well as the combination method were very similar, and all with a midiling result. The balanced random forest classifier method performed considerably better than the previously mentioned methods but still not as good as the easy ensemble adaboost classifier. The easy ensemble was without a doubt the most effective at predicting credit card risk.
