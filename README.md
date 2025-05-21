# Predictive Analysis for Customer Churn

## Overview

This project applies various machine learning algorithms to predict customer churn in the telecommunications industry. The primary goal is to empower telecom companies to proactively identify customers likely to leave, enabling targeted retention strategies and minimizing revenue loss. The project was completed as part of the "Fundamentals of Machine Learning" course in the M.Tech AI program at IIT Hyderabad.

## Dataset

The dataset includes a range of behavioral, demographic, and service-related features:
- Call Failure
- Complaints
- Subscription Length
- Charge Amount
- Seconds of Use
- Frequency of Use
- Frequency of SMS
- Distinct Called Numbers
- Age Group
- Tariff Plan
- Status
- Age
- Customer Value
- Churn (target variable: 0 = retained, 1 = churned)

## Methodology

**Data Preprocessing**
- Feature selection to retain relevant predictors.
- Splitting data into features (X) and target (y).
- 80-20 train-test split for unbiased evaluation.
- Feature normalization using StandardScaler.

**Model Implementation**
- Implemented and tuned multiple models:
  - Deep Neural Network (4 hidden layers, Leaky ReLU, Adam optimizer, early stopping)
  - Random Forest (100 trees, Gini impurity)
  - Logistic Regression
  - SVM (RBF kernel)
  - KNN
  - Naive Bayes
  - LDA
  - Decision Tree

**Evaluation**
- Metrics: Accuracy, Precision, Recall, F1-Score, ROC-AUC.
- Error analysis using confusion matrices.
- Comparative visualization of model performance.

## Results

- **Random Forest** achieved the best results: 95% accuracy, 98% ROC-AUC, and strong F1-score, making it the recommended model for churn prediction.
- **Neural Network** and **SVM** also performed well, with high accuracy and ROC-AUC.
- **Logistic Regression** offered good interpretability and efficiency (88% accuracy, 93% ROC-AUC).
- **Naive Bayes** had high recall but low precision, leading to more false positives.

## Key Insights

- Effective feature selection and normalization are critical for model performance.
- Random Forest is robust and accurate for churn prediction, but simpler models like Logistic Regression are viable for scenarios prioritizing interpretability and speed.
- Multiple evaluation metrics provide a comprehensive view of model strengths and weaknesses.

## Limitations & Future Work

- Apply models to larger, more complex, and imbalanced real-world datasets.
- Explore ensemble methods, advanced deep learning, and AutoML.
- Investigate model interpretability for actionable business insights.

## How to Run

1. Clone this repository.
2. Install dependencies from `requirements.txt`.
3. Place the dataset CSV in the project directory.
4. Run the main notebook or script to preprocess data, train models, and evaluate results.

## Authors

- Aashish Singh (M.Tech AI, IIT Hyderabad)
- Prof. Soumya Jana (Supervisor, IIT Hyderabad)

---

For more details, see the full project report.
