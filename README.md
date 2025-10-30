# Employee-Attrition-Prediction
This is a machine learning project using XGBClassifier.

Overview:
The goal of this project was to predict which employees are likely to leave the company. I began with Logistic Regression as a baseline but noticed that the data was highly imbalanced. To address this, I used SMOTE for oversampling and switched to XGBoost (XGBClassifier), which handles imbalance effectively through the scale_pos_weight parameter.

Process:
Data Preprocessing: Removed Employee_ID, label-encoded categorical columns.
Balancing: Applied SMOTE to generate synthetic samples for the minority class.
Model: Trained XGBClassifier(scale_pos_weight=4.32, random_state=42) on resampled data.
Evaluation: Used accuracy, precision, recall, F1-score, and a confusion matrix for performance assessment.

Results:
Accuracy: 0.70
F1 (Attrition=1): 0.26
Confusion Matrix:[[162  41][ 34  13]]

Future improvements:
May include hyperparameter tuning, feature engineering etc.
