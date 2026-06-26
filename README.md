# NFL Draft Pick Prediction

Predicting NFL Draft selections using machine learning, feature engineering, and ensemble learning techniques.

**Notebook:**
[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1RfwbskPQbXNsIz0yd5C8jucG8bt7ZVCm#scrollTo=9MyLy3x3RfBj)

---


## Repository Structure

```
nfl-draft-prediction/

├── notebook/
│   └── NFL_Draft_Prediction.ipynb
│
├── experiments/
│   ├── feature_engineering.ipynb
│   ├── feature_selection.ipynb
│   ├── hyperparameter_tuning.ipynb
│   └── ensembling.ipynb
│
├── data/
│   ├── train.csv
│   ├── test.csv
│   └── sample_submission.csv
│
├── figures/
│   ├── input.jpg
│   ├── distribution.png
│   └── correlation.png
│
├── output/
│   └── submission.csv
│
├── requirements.txt
└── README.md
```

---

## Overview

This project explores the application of supervised machine learning techniques to predict NFL draft selections from player combine statistics, physical attributes, collegiate background, and engineered performance metrics.

The project follows a complete machine learning workflow including:

* Data preprocessing
* Exploratory Data Analysis (EDA)
* Feature Engineering
* Feature Selection
* Hyperparameter Optimization
* Ensemble Learning
* Performance Evaluation

The final solution combines multiple gradient boosting and tree-based models through performance-weighted averaging using 5-Fold Cross Validation.

---
## Project Workflow

```
Raw Dataset
      │
      ▼
Data Cleaning
      │
      ▼
Exploratory Data Analysis
      │
      ▼
Feature Engineering
      │
      ▼
Feature Selection
      │
      ▼
Model Training
      │
      ▼
Hyperparameter Tuning
      │
      ▼
Ensemble Learning
      │
      ▼
Prediction
```

---



## Models

The following models were trained and evaluated using 5-Fold Cross Validation.

| Model         | Validation AUC |
| ------------- | -------------: |
| CatBoost      |     **0.8517** |
| Random Forest |         0.8464 |
| XGBoost       |         0.8412 |
| LightGBM      |         0.8391 |

The final submission uses **performance-weighted ensemble averaging**, where each model contributes proportionally to its validation performance.

Overall Validation AUC:

**0.84 – 0.85**

---


## Techniques Used

* Exploratory Data Analysis
* Missing Value Imputation
* Feature Engineering
* Feature Selection
* Target Encoding
* Hyperparameter Optimization
* 5-Fold Cross Validation
* Performance-Weighted Ensembling
* Gradient Boosting
* Tree-Based Learning

---
