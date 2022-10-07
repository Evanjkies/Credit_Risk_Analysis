# Credit_Risk_Analysis

## Overview of the Analysis
The purpose of this analysis was to test a machine learning program in its ability to accurately determine credit card risk using RandomOverSampler and SMOTE algorithims for oversampling, and the ClusterCentroids algorithim for undersmapling. The model was also testied using the BalancedRandomForestClassifier and the EasyEnsembleClassifier to predict credit credit risk. The various methods of using the data to help the program learn were evaluated at the end to determine which was the most effective.

## Results

### Naive Random Oversampling
![Naive](https://user-images.githubusercontent.com/107013312/194456273-203d23a2-a630-442c-b4ca-04f9cf0fd6b7.png)

- Balanced Accuracy = .637
- High Risk Percision = .01
- Low Risk Percision = 1.00

### SMOTE Oversampling
![SMOTE](https://user-images.githubusercontent.com/107013312/194456288-555a45b7-c6f1-4d95-8404-7fb52ed4f41f.png)

- Balanced Accuracy = .630
- High Risk Percision = .01
- Low Risk Percision = 1.00

### Cluster Centroids Undersmapling
![Undersampling](https://user-images.githubusercontent.com/107013312/194456303-90ab3238-bf7a-4bcd-a429-a83052551ea1.png)

- Balanced Accuracy = .522
- High Risk Percision = .01
- Low Risk Percision = 1.00

### Combination (Over and Under) Sampling
![Combination](https://user-images.githubusercontent.com/107013312/194456328-6ebb1bb2-eaa1-47c2-83f7-b404547eb638.png)

- Balanced Accuracy = .653
- High Risk Percision = .01
- Low Risk Percision = 1.00

### Balanced Random Forest Classifier
![Balanced_Random_Forest_Classifier](https://user-images.githubusercontent.com/107013312/194456344-b4c27b95-b33d-456e-8b84-cad8219a70c5.png)

- Balanced Accuracy = .789 
- High Risk Percision = .03
- Low Risk Percision = 1.00

### Easy Ensemble AdaBoost Classifier
![Easy_Ensemble](https://user-images.githubusercontent.com/107013312/194456351-5eef6aa3-10cf-4f12-9efe-8bed9e0c9ba9.png)

- Balanced Accuracy = .932
- High Risk Percision = .09
- Low Risk Percision = 1.00

## Summary
The under sampling model had the worst accuracy score, followed by the oversampling methods and the combination method, all of which had middling scores. The ensemble methods were both considerably better but the easy ensemble accuracy score when determining loan risk was clearly the best. All of the methods were considerably more percise when predicting low risk determinations compared to high risk, but the easy ensemble classifier algorithim was the clear winner in this category as well. 

### Recommendation
A case could be made that the easy ensemble method could be reccommended for actual use based on the fact that it is prediciting ~93% of all the risk determinations correctly, and because when it is wrong, it is erroring on the safe side, which is assuming more often than is actually the case that an applicant is high risk. 
