# SWYNEX Machine Learning Model Comparison

## Overview

This project was developed as part of a machine learning task for **SWYNEX Technologies**.

The objective of this project is to train and compare two suitable machine learning classification models using the **Breast Cancer Wisconsin dataset** and determine which model performs better based on multiple evaluation metrics.

## Objective

The main objectives of this project are:

- Load and explore the dataset.
- Perform basic data quality checks.
- Split the dataset into training and testing sets.
- Train two different machine learning classification models.
- Evaluate both models using appropriate performance metrics.
- Compare the results and identify the better-performing model.

## Dataset

The project uses the **Breast Cancer Wisconsin dataset** available through Scikit-learn.

- Samples: **569**
- Features: **30**
- Missing values: **0**
- Duplicate rows: **0**

The task is a binary classification problem.

## Machine Learning Models

Two classification models were trained:

### 1. Logistic Regression

Logistic Regression was implemented using a pipeline with:

- StandardScaler
- Logistic Regression
- Maximum iterations: 1000

### 2. Random Forest Classifier

Random Forest was implemented using:

- 200 decision trees
- Random state: 42

## Evaluation Metrics

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- Confusion Matrix
- Classification Report

## Results

| Metric | Logistic Regression | Random Forest |
|---|---:|---:|
| Accuracy | 98.25% | 95.61% |
| Precision | 98.61% | 95.89% |
| Recall | 98.61% | 97.22% |
| F1-score | 98.61% | 96.55% |
| ROC-AUC | 99.54% | 99.31% |

## Conclusion

Based on the experimental results, **Logistic Regression performed better overall than Random Forest** on the selected test set.

Logistic Regression achieved higher accuracy, precision, F1-score, and ROC-AUC, while Random Forest achieved a slightly lower overall performance.

Therefore, Logistic Regression was selected as the better-performing model for this particular experiment.

This result demonstrates that a simpler machine learning model can outperform a more complex ensemble model when the dataset is well suited to its decision boundary. However, the conclusion is specific to the dataset, preprocessing approach, train-test split, and model configurations used in this experiment.

## Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Repository Contents

```text
SWYNEX-Machine-Learning-Model/
│
├── Machine_Learning_Model_Comparison.ipynb
├── model_comparison.csv
├── requirements.txt
├── README.md
│
└── results/
    └── confusion_matrices.png
```

## How to Run

Clone the repository and install the required dependencies:

```bash
pip install -r requirements.txt
```

Then open the Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```text
Machine_Learning_Model_Comparison.ipynb
```

Run the notebook cells sequentially to reproduce the analysis and model comparison.

## Author

**Shreya Kumari**

Developed as part of a machine learning task for **SWYNEX Technologies**.
