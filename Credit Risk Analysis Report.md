# Credit Risk Analysis Report

## Overview

This credit risk analysis report aims to identify a model that can be utilized in automating the bank's loan instant approval system. The data that was used to train and evaluate the models included certain demographic information, but focused on high-level industry-standard information such as loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt.

The model's development started with a simple logistic regression model, but needed some oversampling in order to perform at an acceptable rate. The comparison of the scores below explain in greater detail the need for the oversampling. 


## Results


* Model 1:
  * `Accuracy Score:` 0.9442676901753825

  * `Precision Score:` 1.00 (Healthy) / 0.87 (High-Risk)

  * `Recall Score:` 1.00 (Healthy) / 0.89 (High-Risk)



* Model 2:
  * `Accuracy Score:` 0.9959744975744975

  * `Precision Score:` 1.00 (Healthy) / 0.87 (High-Risk)

  * `Recall Score:` 1.00 (Healthy) / 1.00 (High-Risk)

____
The `Accuracy Score` is fairly straight-forward. This score is the rate at which the model correctly predicted the outcome of the loan based on the data that was given to the model.

The `Precision Score` notes the percentage of the loans were correctly predicted to be healthy or high-risk.

The `Recall Score` is the score that shows just how well the model performs. This is the score that we should be concerned with since it is the score that shows how many high-risk applicants the model would approve for loans. 

## Summary

In summary, the recall score for this model demonstrates that the model correctly sorts with virtual perfection any false positives. Said another way, this model essentially eliminates high-risk applicants from being approved for a loan. 

I recommend using the second model for commercial use. With an accuracy score of 99.6% and a recall score of 1.00 on high-risk applicants, this model is ready to be deployed. 
