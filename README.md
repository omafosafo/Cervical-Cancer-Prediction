# Cervical Cancer Prediction model
In this project, I trained a support vector machine (SVM) classifiers using the Cervical
Cancer dataset in the UCI Machine Learning Repository.

Features:
I selected only continuous variables as defined in the dataset.

Target variable:
“Biopsy” (binary)

For Data partitioning:
70% training and 30% test data
To ensure even distribution of dataset across the training and test set, I randomly shuffled before partitioning

Data pre-processing:
First, imputed missing values with medians
Then, scaled each feature to be zero mean and unit variance. Pre-processed the training and test data separately to avoid data leakage

Hyperparameter tuning:
For hyperparameter tuning: I tried these strategies ‘linear’, ‘poly’, ‘rbf’, ‘sigmoid’, Set class_weight = ’balanced’ (due to the class imbalance in this dataset)

Final model training and evaluation:
I Trained the final SVM model with the chosen kernel on the entire training data
and Evaluated the trained model on the test data. I then printed the performance metrics for the chosen kernel, F1 score, precision, recall, AUC, and balanced accuracy

