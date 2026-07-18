# Breast Cancer Model Comparison

AI Track internship task — comparing two classification models on the same dataset using a fair, single train-test split.

## Overview

This project trains and evaluates two classifiers — **Logistic Regression** and **Decision Tree** — on the Breast Cancer Wisconsin dataset (569 samples, 30 features, binary classification: malignant vs benign).

## Results

| Metric | Logistic Regression | Decision Tree |
|---|---|---|
| Accuracy | 98.25% | 91.23% |
| Recall (malignant) | 97.6% | 92.9% |

**Logistic Regression performed better across every metric**, with notably fewer missed cancer cases (1 vs 3 false negatives), which matters most in a medical diagnosis context.

## Bonus Work

- 5-fold cross-validation to confirm result stability
- Random Forest as a third model (95.6% accuracy)
- Hyperparameter tuning of Decision Tree's `max_depth` (improved to 93.86%)

## Setup

```bash
pip install -r requirements.txt
```

Then open `model_comparison_Ghania.ipynb` in Jupyter or VS Code.

## Tools Used

Python, scikit-learn, pandas, matplotlib
