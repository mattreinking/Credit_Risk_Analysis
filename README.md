# Credit_Risk_Analysis

## Overview of the Project
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. This project is about employing different techniques to train and evaluate models with unbalanced classes. Jill asks you to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling. Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, the data is oversampled using the RandomOverSampler and SMOTE algorithms, and undersampled the data using the ClusterCentroids algorithm. Then, a combinatorial approach is used for over- and undersampling using the SMOTEENN algorithm. Next is comparing two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk.

### Resources
- Visual Studio Code
- Libraries: imbalanced-learn, scikit-learn
- Algorithms: RandomOverSampler, SMOTE, ClusterCentroids, SMOTEENN
- LoanStats_2019Q1.csv  

### Metrics
- Accuracy: The reliabilty of the predictive scoring.
- pre = Precision: The reliability of positive classification. Low precision equates to a large number of false positives.
- rec = Recall: The ability to find all positive samples. Low recall equates to a large number of false negatives.
- spe = Specificity: The recall of negative values. What portion of negative predictions are true.
- f1 = F1 Score: Weighted average of the Recall and Precision rate.
- geo = Geometric Mean: Analyzes algorithmic performance on a score of 0.0-1.0.
- iba = Index Balanced Accuracy: Evaluates the learning processes in two-class imbalanced domains.
- sup = Support: Number of occurrences of each y_true value.

## Results
RandomOverSampler  
![image](https://user-images.githubusercontent.com/86776606/199567126-8476a14f-7f34-4201-9140-b4105ba0e822.png)
![image](https://user-images.githubusercontent.com/86776606/199531718-babff12d-00d0-4a29-b629-ac99cbb79740.png)  
- The RandomOverSampler has an accuracy score of 64%, total precision score of 99% and total recall score of 58%


SMOTE Oversampling  
![image](https://user-images.githubusercontent.com/86776606/199567288-dc8734f4-7f75-450b-9d58-d795f66e2266.png)
![image](https://user-images.githubusercontent.com/86776606/199531987-0e5653ed-ffda-47ef-90a8-2ad9d7c3d276.png)  
- The SMOTE Oversampling has an accuracy score of 66%, total precision score of 99% and total recall score of 69%


ClusterCentroid Resampler  
![image](https://user-images.githubusercontent.com/86776606/199567423-552aaf73-e628-48a4-bd39-fef68410e2ef.png)
![image](https://user-images.githubusercontent.com/86776606/199532430-6648e548-8ff6-44ce-8ab9-a65f7a797307.png)  
- The ClusterCentroid Resampler has an accuracy score of 66%, total precision score of 99% and total recall score of 69%


SMOTEENN  
![image](https://user-images.githubusercontent.com/86776606/199567491-a19580fb-9a95-4437-afe4-c3315d1a1668.png)
![image](https://user-images.githubusercontent.com/86776606/199532699-884ab1e4-c7c7-4a63-a231-8981bacc859a.png)  
- The SMOTEENN has an accuracy score of 66%, total precision score of 99% and total recall score of 69%


BalancedRandomForestClassifier  
![image](https://user-images.githubusercontent.com/86776606/199567610-c1827e2b-d6c1-4e84-8cfc-9f1153a98ca1.png)
![image](https://user-images.githubusercontent.com/86776606/199542415-f88400c1-5a30-4529-a81a-8491efda2ab7.png)  
- The BalancedRandomForestClassifier has an accuracy score of 83%, total precision score of 99% and total recall score of 90%


EasyEnsembleClassifier  
![image](https://user-images.githubusercontent.com/86776606/199567667-d8e4dd05-519d-4ac9-9238-80d16d193549.png)
![image](https://user-images.githubusercontent.com/86776606/199542546-68265f9b-c8f0-4ec1-8c23-91fcdac437f8.png)  
- The EasyEnsembleClassifier has an accuracy score of 93%, total precision score of 99% and total recall score of 94%

## Summary
The first group of four resampling models were used to predict which loans are at highest risk. All the resampling models had a 99% precision score meaning all good candidates were predicted correctly 99% of the time. While the precision score is near perfect, all four models failed to even reach an accuracy score of 70%. None of the resampling models would be recommended to use for the lending company to calculate credit risk.

The last two were machine learning models used to reduce bias when calculating credit risk. Both machine learning models excelled in calculations with the lowest accuracy score only being 83%. Both models were very effective with neither precision or recall scores never falling below 90%. Peer-to-Peer would do well with either model. My recommendation would be to utilize the EasyEnsembleClassifier machine learning model for predicting credit card risk. EasyEnsembleClassifier had an incredible accuracy score of 93%. Being able to make predictions at such an exceptional degree will make credit decisions much easier to make.
