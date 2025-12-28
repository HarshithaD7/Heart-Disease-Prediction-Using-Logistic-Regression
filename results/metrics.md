Model Evaluation Metrics

1. Model Details
* Model Type: Logistic Regression
* Problem Type: Binary Classification
* Classes:
=> 0 → No heart disease
=> 1 → Presence of heart disease
* Total Samples: 1126

2. Training Configuration
* Feature scaling: Applied
* Train–test split: Used
* Solver: Scikit-learn default
* Evaluation method: Test set evaluation

3. Overall Accuracy
84.90%

4. Classification Report
|               Class | Precision | Recall | F1-Score |  Support |
| ------------------: | --------: | -----: | -------: | -------: |
|      0 (No Disease) |      0.85 |   0.99 |     0.92 |      951 |
| 1 (Disease Present) |      0.61 |   0.08 |     0.14 |      175 |
|        **Accuracy** |           |        | **0.85** | **1126** |
|       **Macro Avg** |      0.73 |   0.54 |     0.53 |     1126 |
|    **Weighted Avg** |      0.82 |   0.85 |     0.80 |     1126 |

4. Confusion Matrix Summary
* True Negatives: High
* True Positives: Low
* False Negatives: High
* False Positives: Low

This indicates strong performance on the negative class and weak detection of positive heart disease cases.
