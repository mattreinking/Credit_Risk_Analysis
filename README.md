# Credit_Risk_Analysis

## Overview of the Project
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. This project is about employing different techniques to train and evaluate models with unbalanced classes. Jill asks you to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling. Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, the data is oversampled using the RandomOverSampler and SMOTE algorithms, and undersampled the data using the ClusterCentroids algorithm. Then, a combinatorial approach is used for over- and undersampling using the SMOTEENN algorithm. Next, two new machine learning models are comapred that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk.

### Resources
- Visual Studio Code
- Libraries: imbalanced-learn, scikit-learn
- Algorithms: RandomOverSampler, SMOTE, ClusterCentroids, SMOTEENN
- LoanStats_2019Q1.csv  

## Results
RandomOverSampler  
![image](https://user-images.githubusercontent.com/86776606/199531718-babff12d-00d0-4a29-b629-ac99cbb79740.png)

SMOTE Oversampling  
![image](https://user-images.githubusercontent.com/86776606/199531987-0e5653ed-ffda-47ef-90a8-2ad9d7c3d276.png)

ClusterCentroid Resampler  
![image](https://user-images.githubusercontent.com/86776606/199532430-6648e548-8ff6-44ce-8ab9-a65f7a797307.png)

SMOTEENN  
![image](https://user-images.githubusercontent.com/86776606/199532699-884ab1e4-c7c7-4a63-a231-8981bacc859a.png)


## Suammry
