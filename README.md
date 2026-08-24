# Customer Churn Prediction

## Overview

This project develops a machine learning model to predict customer churn using the Telco Customer Churn dataset.

The project follows an end-to-end machine learning workflow, including:

- Data cleaning
- Exploratory Data Analysis (EDA)
- Feature preprocessing
- Train-test splitting
- Logistic Regression
- Decision Tree
- Random Forest
- Stratified 5-Fold Cross-Validation
- Hyperparameter tuning using GridSearchCV
- Model evaluation
- Confusion Matrix
- ROC Curve
- Feature Importance
- Model saving and reloading

## Dataset

The project uses the Telco Customer Churn dataset.

The dataset is not included in this repository. It should be obtained separately and placed in the project directory before running the notebook.

## Machine Learning Models

Three classification models were evaluated:

1. Logistic Regression
2. Decision Tree
3. Random Forest

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC

Five-fold stratified cross-validation and hyperparameter tuning were also performed.

## Final Model

The tuned Random Forest model was selected based on F1-score.

### Final Test-Set Results

| Metric | Score |
|---|---:|
| Accuracy | 75.94% |
| Precision | 53.23% |
| Recall | 77.01% |
| F1 Score | 62.95% |
| ROC-AUC | 84.10% |

Recall and F1-score were given particular importance because identifying customers who may churn is important for customer retention.

## Exploratory Data Analysis

The analysis examined relationships between customer churn and:

- Contract type
- Internet service
- Payment method
- Tenure
- Monthly charges
- Total charges

The analysis found that month-to-month contracts, shorter tenure, higher monthly charges, fiber optic service, and electronic-check payment were associated with higher churn rates in this dataset.

These relationships represent associations in the dataset and should not be interpreted as causal relationships.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Joblib
- Jupyter Notebook

## Project Structure

customer-churn-prediction/
│
├── customer_churn_prediction.ipynb
├── README.md
├── requirements.txt
└── .gitignore

## Conclusion

This project demonstrates an end-to-end customer churn prediction workflow using Python and Scikit-learn.

The tuned Random Forest model achieved a recall of 77.01% and an ROC-AUC of 84.10% on the test set.

The results demonstrate why model evaluation should not rely on accuracy alone, particularly when the target variable is imbalanced.
