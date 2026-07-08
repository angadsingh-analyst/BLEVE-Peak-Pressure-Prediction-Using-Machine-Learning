# BLEVE Peak Pressure Regression

## Project Overview

This project builds a machine learning regression pipeline to predict peak overpressure from Boiling Liquid Expanding Vapour Explosion (BLEVE) simulation data. The goal is to estimate target pressure at different sensor locations around a rigid obstacle using physical, geometric and sensor-position variables.

The project demonstrates an end-to-end predictive analytics workflow: data cleaning, leakage-safe preprocessing, physics-informed feature engineering, model comparison, ensemble modelling, and explainable AI interpretation.

## Methods

- Cleaned and prepared structured simulation data with physical, geometric and sensor-position variables.
- Engineered 25 physics-informed features, including tank-volume measures, energy proxies, sensor distances, obstacle-related features and scaled-distance variables.
- Compared multiple regression models, including linear baselines, Random Forest, Gradient Boosting, XGBoost, LightGBM and MLPRegressor.
- Selected a weighted ensemble combining Gradient Boosting and LightGBM with target transformation.
- Used explainability methods including feature importance, permutation importance, partial dependence and SHAP-style interpretation to assess model behaviour.

## Results

- Final weighted ensemble validation MAPE: **0.0997**
- Public benchmark MAPE: **0.161348**
- Private benchmark MAPE: **0.155453**
- Baseline benchmark MAPE: **0.252786**
- Strongest features included scaled sensor distance, sensor location and obstacle-relative distance, aligning with expected blast-wave behaviour.

## Tools and Libraries

- Python
- pandas
- NumPy
- scikit-learn
- XGBoost
- LightGBM
- SHAP
- Matplotlib
- Seaborn
- SciPy

## Repository Structure

```text
.
├── main_portfolio.ipynb
├── README.md
├── requirements.txt
└── .gitignore
```

## Data Availability

This private repository includes the original assessment data files for personal reproducibility. These files should not be redistributed publicly.

## How to Run

Place the required data files in the project directory or upload them when prompted by the notebook:

```text
train.csv
test.csv
sample_prediction.csv
```

Then open `main_portfolio.ipynb` in Jupyter Notebook or Google Colab and run the cells in order.

## Portfolio Note

This repository is a cleaned portfolio version of a machine learning coursework project. Personal identifiers, academic declaration files, assignment submission documents and restricted dataset files have been removed.
