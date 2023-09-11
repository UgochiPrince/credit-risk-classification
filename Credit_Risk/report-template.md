# Module 12 Report Template

## Overview of the Analysis
The purpose of this analysis is to evaluate machine learning models for credit risk assessment. Specifically, we aimed to predict credit risk for loans based on various financial and borrower-related features. This analysis is essential for making informed lending decisions, as it helps identify high-risk loans that may result in default.

### Data Overview
The dataset used for this analysis contains information on loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, total debt, and loan status (0 for healthy loans and 1 for high-risk loans).
We performed credit risk analysis using machine learning techniques to predict loan statuses.

### Stages of the Analysis
-Data Preparation: We loaded and preprocessed the dataset, including separating features (X) and the target variable (y).

-Model Training: We trained two machine learning models: one on the original data and another on resampled data to address class imbalance. We used Logistic Regression as the classification algorithm.

-Model Evaluation: We evaluated both models using accuracy, precision, recall, and the confusion matrix to assess their performance.

## Results

### Original Data Model
- Balanced Accuracy Score: 0.9520
- Precision (0 - Healthy Loan): 1.00
    - Recall (0 - Healthy Loan): 0.99
    - F1-Score (0 - Healthy Loan): 1.00
- Precision (1 - High-Risk Loan): 0.85
    - Recall (1 - High-Risk Loan): 0.91
    - F1-Score (1 - High-Risk Loan): 0.88

### Resampled Data Model
- Balanced Accuracy Score: 0.9937
- Precision (0 - Healthy Loan): 1.00
    - Recall (0 - Healthy Loan): 0.99
    - F1-Score (0 - Healthy Loan): 1.00
- Precision (1 - High-Risk Loan): 0.84
    - Recall (1 - High-Risk Loan): 0.99
    - F1-Score (1 - High-Risk Loan): 0.91

## Summary

In summary, here are the key findings and recommendations:

- Original Data Model: This model performs reasonably well in predicting high-risk loans (precision: 0.85) but slightly less optimally in identifying them (recall: 0.91). The model's overall accuracy is 95.20%, which is good but may benefit from improvement in predicting high-risk loans. However, this model is well-balanced and can be used with confidence.

- Resampled Data Model: The model trained on resampled data excels in predicting both healthy and high-risk loans. It achieves near-perfect precision and recall for healthy loans and high-risk loans, resulting in an accuracy of 99.37%. This model outperforms the original data model significantly and is recommended for use by the company.

The choice of the model to use depends on the company's specific goals and risk tolerance. If the company prioritizes identifying high-risk loans accurately and minimizing false negatives (loan defaults), the resampled data model is the best choice due to its exceptional performance. However, if a balance between performance and simplicity is preferred, the original data model remains a suitable option with good overall performance.

In conclusion, considering the significant improvement in performance achieved by the model trained on resampled data, we recommend adopting the resampled data model for credit risk assessment to make more informed lending decisions while mitigating the risk of loan defaults.




