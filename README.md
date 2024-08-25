Titanic Survival Prediction: A Machine Learning Approach

1. Introduction

The goal of this project was to predict the survival of passengers on the Titanic using machine learning techniques. The dataset provided contained information about passengers, including their age, sex, class, fare, and whether they survived.

2. Data Exploration and Preprocessing

2.1 Initial Exploration

We began by exploring the dataset using pandas and matplotlib to understand the distribution of features and identify potential patterns. Histograms and heatmaps were used to visualize the data.

2.2 Handling Missing Values

Missing values in the 'Age' and 'Embarked' columns were handled using imputation and one-hot encoding, respectively. The 'Age' column was imputed using the mean strategy, while 'Embarked' was one-hot encoded to create dummy variables.

2.3 Feature Engineering

We created a new feature called 'FamilySize' by combining the 'SibSp' (number of siblings/spouses aboard) and 'Parch' (number of parents/children aboard) columns. This feature was intended to capture the potential impact of family size on survival.

2.4 Dropping Irrelevant Features

Irrelevant features such as 'PassengerId', 'Name', 'Ticket', and 'Cabin' were dropped from the dataset as they were not expected to contribute significantly to the prediction task.

3. Model Selection and Evaluation

3.1 Logistic Regression

We initially used a logistic regression model as a baseline. The model was trained on the preprocessed training data and evaluated on the test data. The accuracy score and classification report were used to assess the model's performance.

3.2 K-Nearest Neighbors (KNN)

A KNN classifier was also trained and evaluated. The number of neighbors (k) was set to 5. The accuracy score and classification report were again used for evaluation.

3.3 Support Vector Machine (SVM)

An SVM classifier was trained and evaluated, providing another perspective on the problem.

3.4 Random Forest

A Random Forest classifier was trained and evaluated, leveraging the power of ensemble learning.

3.5 Hyperparameter Tuning (Logistic Regression)

To improve the performance of the logistic regression model, we performed hyperparameter tuning using GridSearchCV. The grid search explored different combinations of penalty, C (regularization strength), and solver. The best hyperparameters were selected based on cross-validation accuracy.

4. Results and Discussion

The different models showed varying levels of performance. The logistic regression model with hyperparameter tuning achieved the highest accuracy score. The classification reports provided detailed insights into precision, recall, and F1-score for each class (survived or not survived).

5. Conclusion

This project demonstrated the application of machine learning to predict Titanic passenger survival. The results highlight the importance of data preprocessing, feature engineering, and model selection in achieving accurate predictions. Future work could explore more sophisticated feature engineering techniques or ensemble methods to further improve performance.
