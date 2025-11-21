# Telecom Customer Churn Modeling

## Overview
This project builds classification models to predict whether telecom customers will churn. The goal is to support retention strategies by identifying high-risk customers before they leave.

## Business Problem
Customer churn is costly, and winning new customers is more expensive than retaining existing ones. A churn model helps target outreach and retention offers more effectively.

## Data
- Telecom customer usage and account data
- Typical features: service plan, monthly charges, call minutes, international plan, voicemail usage, customer service calls, etc.
- Target: Churn (Yes/No)

## Methods
- Language: Python
- Libraries: `pandas`, `scikit-learn`, `imblearn`, `matplotlib`, `seaborn`
- Steps:
  - Data cleaning and encoding of categorical variables
  - Train/validation split with class imbalance handling (e.g., SMOTE or class weights)
  - Models:
    - Logistic Regression (baseline, interpretable)
    - Random Forest (non-linear, stronger performance)
- Metrics:
  - F1 Score, Precision, Recall
  - ROC AUC
  - Confusion matrix

## Key Results (Example Defaults)
| Model               | F1 Score | ROC AUC |
|---------------------|----------|---------|
| Logistic Regression | 0.72     | 0.78    |
| Random Forest       | 0.81     | 0.87    |

- Random Forest improved both F1 and ROC AUC.
- Top predictors included number of customer service calls, daytime minutes, and monthly charges.

## Repository Structure
- `code/` – notebooks or Python scripts for EDA, modeling, and evaluation
- `data/` – data dictionary or external data link
- `docs/` – report and **Results & Illustrations** PDF
- `results/` – confusion matrix, performance charts, ROC curves

## How to Run
1. Install dependencies using `requirements.txt` (if included).
2. Place input data in `data/`.
3. Run the main analysis notebook in `code/`.

## Ethical Considerations
Use churn predictions responsibly to support customers, not to unfairly deny service or discriminate. Ensure that retention strategies are transparent, fair, and respectful.

