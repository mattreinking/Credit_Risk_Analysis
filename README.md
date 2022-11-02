# Credit_Risk_Analysis

## Overview of the Project
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. This project is about employing different techniques to train and evaluate models with unbalanced classes. Jill asks you to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling. Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, the data is oversampled using the RandomOverSampler and SMOTE algorithms, and undersampled the data using the ClusterCentroids algorithm. Then, a combinatorial approach is used for over- and undersampling using the SMOTEENN algorithm. Next, two new machine learning models are comapred that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk.

### Resources
- Visual Studio Code
- Libraries: imbalanced-learn, scikit-learn
- Algorithms: RandomOverSampler, SMOTE, ClusterCentroids, SMOTEENN
- LoanStats_2019Q1.csv  

### Metrics
- pre = Precision: The reliability of positive classification
- rec = Recall: The ability to find all positive samples
- spe = Specificity: The recall of negative values. What portion of negative predictions are true
- f1 = F1 Score: Weighted average of the Recall and Precision rate
- geo = Geometric Mean: Analyzes algorithmic performance on a score of 0.0-1.0
- iba = Index Balanced Accuracy: Evaluates the learning processes in two-class imbalanced domains
- sup = Support: Number of occurrences of each y_true value

## Results
RandomOverSampler  
![image](https://user-images.githubusercontent.com/86776606/199531718-babff12d-00d0-4a29-b629-ac99cbb79740.png)  
- 

SMOTE Oversampling  
![image](https://user-images.githubusercontent.com/86776606/199531987-0e5653ed-ffda-47ef-90a8-2ad9d7c3d276.png)  
- 

ClusterCentroid Resampler  
![image](https://user-images.githubusercontent.com/86776606/199532430-6648e548-8ff6-44ce-8ab9-a65f7a797307.png)  
- 

SMOTEENN  
![image](https://user-images.githubusercontent.com/86776606/199532699-884ab1e4-c7c7-4a63-a231-8981bacc859a.png)  
- 

BalancedRandomForestClassifier  
![image](https://user-images.githubusercontent.com/86776606/199542415-f88400c1-5a30-4529-a81a-8491efda2ab7.png)  
- 

EasyEnsembleClassifier  
![image](https://user-images.githubusercontent.com/86776606/199542546-68265f9b-c8f0-4ec1-8c23-91fcdac437f8.png)  
- 

## Summary
