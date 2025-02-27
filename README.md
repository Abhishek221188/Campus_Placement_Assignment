Campus Placement Prediction Project Report

Introduction

Getting students placed in good jobs is one of the most important goals for any educational institution. 
The reputation and yearly admissions of a college or university depend a lot on how well they can place their students in jobs. 
This project aims to predict whether a student will be recruited during campus placements or not, based on various factors like academic performance, work experience, and other attributes.

Dataset and Preprocessing
The dataset used for this project is available on Kaggle and includes information about students' academic scores, 
gender, work experience, and whether they were placed or not. Each row in the dataset represents a student.

Preprocessing Steps

1. Loading the Data: loaded the dataset to start our analysis.
2. Handling Missing Values: found some missing values in the salary column and filled them with 0 because students who were not placed would not have a salary.
3. Encoding Categorical Data: converted categorical data (like gender, education background, etc.) into numbers so that machine learning models can process them.
4. Splitting the Data: divided the dataset into two parts: 70% for training our models and 30% for testing their performance.

Chosen Models and Rationale

Selected a variety of machine learning models to see which one works best for predicting placements:

1. Logistic Regression: This model is simple and good for binary classification tasks (like predicting yes or no).
2. Decision Tree Classifier: This model is easy to understand and visualize.
3. Random Forest Classifier: This model uses multiple decision trees to improve accuracy and prevent overfitting.
4. Support Vector Machine (SVM): This model is effective in high-dimensional spaces and good for classification.
5. k-Nearest Neighbors (k-NN): This model is simple and effective for small datasets.
6. Gradient Boosting Classifier: This model builds trees sequentially to improve accuracy.

Training the Models

Trained each of these models on our training data. During training, we adjusted various settings (hyperparameters) for each model to make them perform better.

Evaluating the Models
Evaluated how well each model performed on the test data using several metrics:

- Accuracy: The percentage of correct predictions.
- Precision: How many of the predicted placements were actually correct.
- Recall: How many of the actual placements were correctly predicted.
- F1-Score: A balance between precision and recall.
- ROC-AUC: Measures the model's ability to distinguish between the classes.

also used confusion matrices to visualize the performance of each model.

voting Classifier
To further improve our predictions, we created a Voting Classifier. This classifier combines the predictions of all the models we trained. 
By taking the "vote" of each model, the Voting Classifier often performs better than individual models.

Confusion Matrices
Plotted confusion matrices for each model to see how well they are predicting placements and non-placements.

Best Performing Model
The Voting Classifier performed the best with an accuracy of 90%, precision of 91%, recall of 89%, F1-score of 90%, and ROC-AUC of 94%.
This model combines the strengths of all the individual models, leading to better overall performance.

Conclusion
By using various machine learning models and combining them with a Voting Classifier, I was able to accurately predict whether students would be placed in campus placements. This approach can help educational institutions improve their placement strategies and assist students in securing jobs.

