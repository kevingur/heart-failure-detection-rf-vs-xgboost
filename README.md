# Heart Failure Detection  
## Random Forest vs XGBoost

Overview

Welcome to my Heart Failure Detection Project!
This repository contains a machine learning project focused on predicting heart failure using clinical patient data. The main objective of the project is to compare the performance of Random Forest and XGBoost models, both in their baseline and tuned versions.

The project follows a structured machine learning workflow, including data splitting, model training, evaluation, and hyperparameter tuning, with a strong focus on generalization performance and overfitting analysis.

⸻

Dataset

The dataset used in this project was obtained from Kaggle and contains demographic features such as age and sex, as well as multiple clinical and medical measurements related to cardiovascular health.
It includes demographic and medical features commonly used for heart failure prediction tasks.

The target variable indicates whether a patient has heart disease (HeartDisease).

The dataset is balanced, and stratified splitting is applied to preserve class distribution across training, validation, and test sets.

https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction
⸻

Methods

The following models are implemented and compared:
	•	Random Forest Classifier
	•	Random Forest Baseline model
	•	Random Forest Tuned model 
  
	•	XGBoost Classifier
	•	XGBoost Baseline model
	•	XGBoost Tuned model 

For baseline models, training and validation (CV) performance are compared to analyze overfitting.
For tuned models, hyperparameter optimization is performed using cross-validation, and final evaluation is conducted on a held-out test set.

⸻

Evaluation Metrics

Model performance is evaluated using multiple metrics to provide a comprehensive analysis:
	•	Accuracy (for baseline comparison)
	•	Precision
	•	Recall
	•	F1-score
	•	Confusion Matrix

Special attention is given to recall and F1-score due to their importance in medical prediction tasks.

⸻

Results
	•	Both baseline models show signs of overfitting, with high training accuracy and lower validation accuracy.
	•	Hyperparameter tuning significantly reduces the accuracy gap between training and test sets. 
	•	The tuned XGBoost model still shows some overfitting, likely due to dataset size and model complexity.
  •	The tuned Random Forest model outperforms XGBoost on this dataset. It may be attributed to the characteristics of the dataset and the limited hyperparameter tuning applied to XGBoost.


Overall, tuning improves generalization performance for both models.

⸻

Requirements

To run the notebook locally, make sure you have the following Python libraries installed:
	•	pandas
	•	numpy
	•	scikit-learn
	•	xgboost
	•	matplotlib

⸻

Acknowledgments

This project was completed as an independent machine learning project to practice model comparison, overfitting analysis, and hyperparameter tuning techniques.

It represents my first end-to-end machine learning project, completed individually.

Feedback and suggestions are always welcome!
