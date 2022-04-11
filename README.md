# Credit_Risk_Analysis

## Project Overview
A peer-to-peer lending services company would like to predict credit risk using machine learning. They would like to see the following:
  - Oversampling of the data using the RandomOverSampler and SMOTE algorithms
  - Undersampling of the data using the ClusterCentroids algorithm 
  - Combination sampling (over and under) using the SMOTEENN algorithm
  - Comparison between the BalancedRandomForestClassifier and EasyEnsembleClassifer machine learning models

## Resources
- Data Source: LoanStats_2019Q1.csv
- Software: Jupyter Notebook 6.4.5

## Results

### RandomOverSampler Oversampling
![alt text](https://github.com/thehatch4815162342/Credit_Risk_Analysis/blob/main/Images/RandomOverSampler.png?raw=true)

  - Accuracy - 65%
  - Precision - 99%
  - Recall - 67%

### SMOTE Oversampling
![alt text](https://github.com/thehatch4815162342/Credit_Risk_Analysis/blob/main/Images/SMOTE.png?raw=true)

  - Accuracy - 63%
  - Precision - 99%
  - Recall - 63%

### ClusterCentroids Undersampling
![alt text](https://github.com/thehatch4815162342/Credit_Risk_Analysis/blob/main/Images/Undersampling.png?raw=true)

  - Accuracy - 59%
  - Precision - 99%
  - Recall - 57%

### Combination Sampling
![alt text](https://github.com/thehatch4815162342/Credit_Risk_Analysis/blob/main/Images/Combo_Sampling.png?raw=true)

  - Accuracy - 64%
  - Precision - 99%
  - Recall - 58%

### BalancedRandomForestClassifier
![alt text](https://github.com/thehatch4815162342/Credit_Risk_Analysis/blob/main/Images/BalancedRandomForestClassifier.png?raw=true)

  - Accuracy - 79%
  - Precision - 99%
  - Recall - 91%

### EasyEnsembleClassifier
![alt text](https://github.com/thehatch4815162342/Credit_Risk_Analysis/blob/main/Images/EasyEnsembleClassifier.png?raw=true)

  - Accuracy - 93%
  - Precision - 99%
  - Recall - 94%


## Summary
All models have weak precision scores, thus they will all flag low risk loans as high risk loans very often. The EasyEnsembleClassifer has the best recall score, which in this case is very important. If a high risk loan is marked as low risk, then the company could lose a good amount of money. Accuracy is pretty low for every model except for EasyEnsembleClassifer as well. Due to precision scores being weak across the board, I can not in good faith recommend any of these models.


