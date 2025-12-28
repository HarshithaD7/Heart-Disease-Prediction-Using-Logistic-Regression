Model Observations and Analysis


1. Dataset Observations

* Total samples: 1126
* Class distribution:
-> No heart disease (0): 951 samples
-> Heart disease present (1): 175 samples
* The dataset is highly imbalanced, with far fewer positive heart disease cases.

2. Model Performance Observations

* The model achieves 84.9% accuracy, which appears high at first glance.
* Accuracy is mainly driven by excellent prediction of non-heart disease cases.
* The recall for heart disease cases is very low (0.08), meaning many positive cases are missed.
* Precision for heart disease cases is 0.61, indicating that when the model predicts disease, it is often correct—but it predicts disease very rarely.

3. Confusion Matrix Interpretation

* Most patients without heart disease are correctly classified.
* A large number of patients with heart disease are misclassified as healthy.
* This behavior is typical when training Logistic Regression on imbalanced medical datasets without class balancing.

4. Key Insights

* Accuracy alone is not sufficient for evaluating medical classification models.
* Recall is more critical for detecting heart disease cases.
* The current model is not reliable for medical diagnosis without further improvement.

5. Limitations

* Severe class imbalance affects model learning.
* Logistic Regression struggles with minority class detection.
* No resampling or class weighting was applied.

6. Recommendations

* Apply class balancing techniques such as SMOTE
* Use class weights in Logistic Regression
* Experiment with advanced models like Random Forest or XGBoost
* Optimize evaluation using recall and F1-score instead of accuracy alone
