# Credit_Risk_Analysis

## Overview 

In this supervised machine learning project, I was tasked with helping a credit risk company. We all know that good loans outnumber risky ones, therefore credit risk has a naturally unbalanced classification issue. I was able to use different techniques to train and evaluate models with unbalanced classes. I then evaluated the performance of these models to determine if they can be used to predict credit risk and help this company evaluate its loan applicants. 

## Resources

Software: Jupyter Notebook
    
Provided Data: [Loan Stars 2019 Q1 Data](data/LoanStats_2019Q1.csv)

Provided Starter Code: [Link](code/starter_code)

## Code
[Credit Risk Resampling](code/credit_risk_resampling.ipynb)
[Credit Risk Ensemble](code/credit_risk_ensemble.ipynb) 

## Results 

### Findings 

Credit Risk Sampling Results:
- Naïve Random Oversampling
    - Balanced Accuracy Score: 0.6438020474515633
    - High Risk Precision Score: 0.01
    - Low Risk Precision Score: 1.00
    - High Risk Recall Score: 0.61
    - Low Risk Recall Score: 0.68
- SMOTE Oversampling
    - Balanced Accuracy Score: 0.640903304043737
    - High Risk Precision Score: 0.01
    - Low Risk Precision Score: 1.00
    - High Risk Recall Score: 0.62
    - Low Risk Recall Score: .066
- Cluster Centroids Undersampling
    - Balanced Accuracy Score: 0.510980577009077
    - High Risk Precision Score: 0.01
    - Low Risk Precision Score: 1.00
    - High Risk Recall Score: 0.57
    - Low Risk Recall Score: 0.45
- SMOTEENN - Combination (Over and Under) Sampling
    - Balanced Accuracy Score: 0.6601460048104233
    - High Risk Precision Score: 0.01
    - Low Risk Precision Score: 1.00
    - High Risk Recall Score: 0.68
    - Low Risk Recall Score: 0.64
- Balanced Random Forest Classifier
    - Balanced Accuracy Score: 0.7875627993924523
    - High Risk Precision Score: 0.04
    - Low Risk Precision Score: 1.00
    - High Risk Recall Score: 0.67
    - Low Risk Recall Score: 0.91
- Easy Ensemble AdaBoost Classifier
    - Balanced Accuracy Score: 0.925427358175101
    - High Risk Precision Score: 0.07
    - Low Risk Precision Score: 1.00
    - High Risk Recall Score: 0.91
    - Low Risk Recall Score: 0.94

### Images 


### Summary & Recommendations

Preforming these classifier tests, we see that each iteration provides results that continually increase their success rate. The first 4 tests yielded results that we preformed left much to be desired for.  The SMOTEENN sampling process looked promising at first bet then I came to the next two and they produced even better results.  

In conclusion the Easy Ensemble AdaBoost Classifier is the best model to use for the credit risk assessment to evaluate loan applicants potential risk. 


