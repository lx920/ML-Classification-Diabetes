# ML-Classification-Diabetes
Use popular ML Classification models on diabetes data set. Compare precision, recall, ROC AUC and confusion matrices\

- Logistic Regression
- Support Vector Machine
- Random Forest

# Data Source:
The data source is from Kaggle: Pima Indian Diabetes Dataset. https://www.kaggle.com/uciml/pima-indians-diabetes-database \

# Data Processing:
There are 9 columns and 768 rows of data. \
Used Median Imputation and KNN imputation on missing entries on data set

# Logistic Regression
Logistic Regression serves as a baseline for classification
Accuracy = 0.805 Precision = 0.707 Recall = 0.617

# Support Vector Machine
SVM with default hyperparameters gives worse classification than Logistic regression\
Applied GridSearch CV to find best Hyperparameters\
C: 100, gamma: Scale, Kernel: Linear\
Tuned Model have: \
Accuracy 0.82, Precision 0.71 Recall 0.68\
\
High compupational cost of SVM prevents me from exploring more in poly and rbf kernels.

# Random Forest
Averaging Classification over 10000 Decision Trees\
Accuracy 0.826 Precision 0.717 Recall 0.702\
Random Forest slightly outperforms SVM in this case.\
RF is the superior model in this case because of less time complexity.
