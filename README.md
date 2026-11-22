# Home Credit Default Risk Prediction

**GCI Global 2026 | Machine Learning Competition**

**Author:** Ahmed Hany

## Project Overview

This project develops a machine-learning pipeline to predict the probability of loan default using the Home Credit Default Risk dataset.

The objective is to identify customers who may experience difficulties repaying their loans, using financial, demographic, and behavioral features.

**Evaluation Metric:** ROC-AUC

## Technologies & Libraries

- Python
- Pandas & NumPy
- Scikit-learn
- LightGBM
- CatBoost
- Optuna
- Matplotlib & Seaborn

## Methodology

### 1. Exploratory Data Analysis
- Missing-value analysis
- Correlation analysis
- Identification of data anomalies
- Analysis of important financial indicators

### 2. Feature Engineering
- Credit-to-income and annuity-to-income ratios
- Age and employment-related features
- External source score combinations
- Credit bureau inquiry features
- Group-based statistical features
- Out-of-fold target encoding
- K-nearest-neighbor target features

### 3. Model Development
- LightGBM gradient boosting
- CatBoost classification
- Stratified cross-validation
- Optuna hyperparameter optimization
- Ensemble learning and prediction blending

### 4. Model Evaluation
Models are evaluated using ROC-AUC, with out-of-fold predictions used to assess generalization performance.

### 5. Submission
Predictions are exported in the required CSV submission format.

## Repository Structure

```text
home-credit-default-risk-prediction/
├── README.md
├── competition_lgbm.py
├── requirements.txt
├── .gitignore
├── notebooks/
│   └── competition_lgbm.ipynb
├── input/
└── output/
```

## Installation

Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/home-credit-default-risk-prediction.git
cd home-credit-default-risk-prediction
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Download the competition datasets and place the required CSV files inside the `input/` directory.

Required files:
- `train.csv`
- `test.csv`
- `sample_submission.csv`

## Reproducibility

- Fixed random seeds.
- Stratified cross-validation.
- Out-of-fold target encoding.
- No external training datasets.
- Reproducible feature engineering.

## Acknowledgments & References

- GCI Global 2026 competition.
- Matsuo-Iwasawa Lab, University of Tokyo, for the original tutorial structure.
- Home Credit Default Risk Kaggle competition.
- Will Koehrsen and Aguiar for publicly shared feature-engineering approaches.

## Author

**Ahmed Hany**

Molecular Biotechnology Student | Machine Learning & Biotechnology Enthusiast

