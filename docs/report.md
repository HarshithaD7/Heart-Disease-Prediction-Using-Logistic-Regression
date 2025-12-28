Heart Disease Prediction Using Logistic Regression Project Documentation

1. Problem Statement

Heart disease is a major health concern, and early identification can significantly reduce complications and mortality.
The objective of this project is to predict the presence of heart disease using patient medical data through a Logistic Regression classification model.

The task is formulated as a binary classification problem where the model predicts whether a patient has heart disease (1) or not (0).

2. Dataset Description
* Total records used: 1126 patients
* Each row represents a single patient
* Target variable:
=> 0 → No heart disease
=> 1 → Presence of heart disease

Class Distribution
* Class 0 (No heart disease): 951 samples
* Class 1 (Heart disease present): 175 samples
This indicates a class imbalance, with significantly fewer positive heart disease cases.

3. Data Preprocessing
The following preprocessing steps were performed:
* Dataset inspection using df.head() and df.info()
* Separation of input features (X) and target variable (y)
* Feature scaling applied to normalize numerical attributes
* Dataset split into training and testing sets using train_test_split

These steps ensured the data was suitable for Logistic Regression modeling.

4. Model Selection
Logistic Regression was selected due to:
* Its effectiveness for binary classification problems
* Interpretability of results
* Suitability for structured medical datasets

The model predicts probabilities which are converted into binary class labels.

5. Model Training
The Logistic Regression model was trained on the training dataset using Scikit-learn.
* Training Details
  -> Algorithm: Logistic Regression
  -> Total samples used: 1126
  -> Model fitting performed using:
      model.fit(X_train, y_train)
  
6. Model Evaluation
Model Accuracy: 0.8490 (84.90%)

Classification Report

|               Class | Precision | Recall | F1-Score |  Support |
| ------------------: | --------: | -----: | -------: | -------: |
|      0 (No Disease) |      0.85 |   0.99 |     0.92 |      951 |
| 1 (Disease Present) |      0.61 |   0.08 |     0.14 |      175 |
|        **Accuracy** |           |        | **0.85** | **1126** |
|       **Macro Avg** |      0.73 |   0.54 |     0.53 |     1126 |
|    **Weighted Avg** |      0.82 |   0.85 |     0.80 |     1126 |

7. Confusion Matrix Analysis
The confusion matrix generated in the notebook shows:

* A high number of True Negatives, indicating correct prediction of patients without heart disease
* A low number of True Positives, showing difficulty in detecting heart disease cases
* The model struggles with positive class prediction due to dataset imbalance

8. Results and Observations
* The model achieves 84.9% accuracy
* Strong performance in predicting absence of heart disease
* Very low recall (0.08) for heart disease cases
* Class imbalance significantly affects the model’s ability to detect positive cases


