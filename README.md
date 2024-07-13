# Diabetes Classification Project

## Overview

This project aims to analyze the diabetes dataset and apply various classification algorithms to determine which model performs best in predicting whether a patient has diabetes based on diagnostic measurements. The classification algorithms used include Logistic Regression, kNN, Decision Tree, Naïve Bayes, and SVM. The models are evaluated on different performance metrics such as accuracy, confusion matrix, and Area Under the ROC Curve (AUC).

## Dataset

The dataset used in this project is originally from the National Institute of Diabetes and Digestive and Kidney Diseases. It consists of several diagnostic measurements for female patients of at least 21 years old. The objective is to predict whether a patient has diabetes (Outcome variable: 0 or 1). The dataset is included in the repository.

### Features:

- `Glucose`: Plasma glucose concentration a 2 hours in an oral glucose tolerance test
- `BloodPressure`: Diastolic blood pressure (mm Hg)
- `SkinThickness`: Triceps skin fold thickness (mm)
- `Insulin`: 2-Hour serum insulin (mu U/ml)
- `BMI`: Body mass index (weight in kg/(height in m)^2)
- `DiabetesPedigreeFunction`: Diabetes pedigree function
- `Age`: Age (years)
- `Outcome`: Class variable (0 or 1)

## Methodology

### Data Preprocessing

- Handle zero values by treating them as NaN and imputing with central tendency measures.
- Apply StandardScaler to the dataset.
- Split the data into training and test sets, maintaining class distribution.

### Exploratory Data Analysis (EDA)

- Perform multivariate analysis using correlation heatmaps and pairplots.
- Use countplots and more visualizations to understand data distribution.
- Plot boxplots to detect outliers.
- Handle outliers using the Interquartile Range (IQR) based capping method.
- Analyze the distribution of data using Q-Q plots.

### Model Training and Evaluation

The following classification algorithms are implemented and evaluated:

- Logistic Regression
- k-Nearest Neighbors (kNN)
- Decision Tree
- Naïve Bayes
- Support Vector Machine (SVM)

### Evaluation Metrics

- Accuracy
- Confusion Matrix
- ROC AUC Score

## Results

The ROC AUC scores of the models are as follows:

| Model                       | ROC AUC Score |
|-----------------------------|---------------|
| Logistic Regression         | 0.8285        |
| k-Nearest Neighbors (kNN)   | 0.8193        |
| Decision Tree               | 0.7333        |
| Gaussian Naive Bayes        | 0.8272        |
| Support Vector Machine (SVM)| 0.8311        |

Among the classification models evaluated, the Gaussian Naive Bayes and SVM Classifier exhibits slightly better performance relative to the other classification models.

## Importance

Projects like this are crucial in the medical industry as they provide a data-driven approach to diagnosing diseases such as diabetes. Early and accurate detection of diabetes can significantly improve patient outcomes and reduce healthcare costs. By leveraging machine learning algorithms, medical professionals can gain insights from diagnostic data, leading to more informed decision-making and personalized treatment plans.
