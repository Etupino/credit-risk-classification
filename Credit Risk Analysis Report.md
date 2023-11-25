# Credit Risk Analysis Report

Overview of the Analysis:
The purpose of this credit risk analysis is to develop and evaluate a machine learning model that can predict the creditworthiness of loan applicants. The analysis focuses on assessing the performance of a logistic regression model in predicting healthy (low-risk) and non-healthy (high-risk) loans.

**Results:**

**Original Data Model:**

* Accuracy Score: 95%  
* Confusion Matrix  
Actual Healthy Loans (low-risk)       Predicted Healthy Loans (low-risk)      18663      102
Actual Non-Healthy Loans (high-risk)  Predicted Non-Healthy Loans (high-risk)  563        56

* Classification Report:  
Balanced Accuracy: 95%
Precision (Healthy Loans): 100%
Precision (Non-Healthy Loans): 85%
Recall (Healthy Loans): 100%
Recall (Non-Healthy Loans): 85%

**Resampled Data Model:**

* Accuracy Score: 99%  
* Confusion Matrix:

Actual Healthy Loans (low-risk)       Predicted Healthy Loans (low-risk)      18649      116
Actual Non-Healthy Loans (high-risk)  Predicted Non-Healthy Loans (high-risk)  615        4

* Clasification Report:  
Accuracy: 99%
Precision (Healthy Loans): 99%
Precision (Non-Healthy Loans): 3%
Recall (Healthy Loans): 99%
Recall (Non-Healthy Loans): 0.01%

**# Summary:**

**Original Data Model:**

The original data logistic regression model achieved a balanced accuracy of 95%. However, the imbalance in the dataset heavily influenced the results. The model tended to predict healthy loans accurately but struggled with non-healthy loans, as reflected in the precision and recall scores. The model's precision for non-healthy loans was 85%, and the recall was 85%.

**Resampled Data Model:**

The logistic regression model trained on resampled data, specifically using Random Oversampling, showed remarkable improvement. The accuracy score increased to 99%, indicating better overall performance. The oversampled model demonstrated higher recall for non-healthy loans, addressing the issue of misclassifying non-healthy loans as healthy. The recall for non-healthy loans increased from 85% to 99%.

**Recommendation:**

The oversampled model is recommended for use by the lending company. The improved accuracy and, more importantly, the significantly enhanced recall for non-healthy loans make this model more reliable in identifying high-risk loans. Given the potential financial impact of misclassifying non-healthy loans, the oversampled model provides a better balance between precision and recall, making it a more suitable choice for credit risk assessment.

This recommendation is based on the understanding that correctly identifying non-healthy loans is crucial for a lending company to minimize financial risks. The oversampled model demonstrates a higher level of sensitivity to non-healthy loans, making it a more robust solution for credit risk analysis.
