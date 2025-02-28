Campus Placement Prediction

🔹 Introduction

📌 Problem Summary

Securing student placements is crucial for educational institutions as it impacts their reputation and admissions. This project predicts whether a student will be placed based on academic performance, work experience, and other factors.

🎯 Dataset & Preprocessing

Dataset: Sourced from Kaggle, it includes academic scores, gender, work experience, and placement status.

Preprocessing Steps:

Data Loading: Imported the dataset for analysis.

Handling Missing Values: Filled missing salary values with 0 for unplaced students.

Encoding Categorical Data: Converted categorical variables into numerical format.

Data Splitting: 70% for training, 30% for testing.

📌 Chosen Models & Rationale

Logistic Regression: Ideal for binary classification.

Decision Tree Classifier: Simple and interpretable.

Random Forest Classifier: Improves accuracy with multiple trees.

Support Vector Machine (SVM): Effective in high-dimensional spaces.

k-Nearest Neighbors (k-NN): Works well with small datasets.

Gradient Boosting Classifier: Enhances accuracy through sequential learning.

🔹 Model Training & Evaluation

Trained each model on the dataset and optimized hyperparameters.

Evaluation Metrics:

Accuracy – Overall correctness of predictions.

Precision – Proportion of correct placement predictions.

Recall – Correctly identified placed students.

F1-Score – Balance between precision and recall.

ROC-AUC – Measures classification performance.

Used confusion matrices to visualize model performance.

🏆 Best Performing Model

The Voting Classifier achieved the highest accuracy of 90%, with:

Precision: 91%

Recall: 89%

F1-Score: 90%

ROC-AUC: 94%

This ensemble model combined multiple classifiers to improve prediction reliability.

📌 Conclusion

By leveraging machine learning models, this project accurately predicts student placements. The insights gained can help institutions enhance their placement strategies, ultimately increasing job opportunities for students.
