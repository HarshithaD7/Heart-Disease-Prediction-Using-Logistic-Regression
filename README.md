Heart Disease Prediction Using Logistic Regression

1. Project Description:
* This project predicts the presence of heart disease using a Logistic Regression model implemented and executed in a Kaggle Notebook environment.
* The model uses structured medical data to classify whether a patient has heart disease (1) or not (0).
* The notebook covers the complete machine learning workflow including data preparation, model training, evaluation, and prediction.

2. Objectives:
* Load and analyze heart disease medical dataset
* Preprocess and scale patient health attributes
* Build a Logistic Regression classification model
* Evaluate model performance using accuracy and classification metrics
* Predict heart disease presence for unseen patient data

3. Dataset
* Total samples: 1126 patient records
* Target variable:
=> 0 → No heart disease
=> 1 → Presence of heart disease

4. Class Distribution
* No heart disease: 951 samples
* Heart disease present: 175 samples

5. Source Code
* Complete implementation is provided as a Jupyter Notebook inside the src/ folder.

6. Execution Environment
* Platform: Kaggle Notebooks
* Language: Python
* Libraries:
-NumPy
-Pandas
-Matplotlib
-Scikit-learn
All execution is performed within the Kaggle environment.

7. Results
* Model accuracy: 84.90%
* Strong performance in predicting patients without heart disease
* Very low recall (0.08) for heart disease cases due to class imbalance
* Confusion matrix and classification report are generated for detailed evaluation
* Detailed results are available in the results/ folder:

