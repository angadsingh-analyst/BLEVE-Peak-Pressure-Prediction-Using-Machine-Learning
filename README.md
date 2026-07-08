# BLEVE Peak Pressure Prediction Using Machine Learning

This project develops a machine learning regression pipeline to predict peak overpressure from BLEVE-related experimental and simulation data. The aim was to build an accurate predictive model, compare multiple regression approaches, and generate final predictions for unseen test data.

The project demonstrates skills in data preprocessing, feature engineering, regression modelling, ensemble learning, model evaluation and explainable machine learning.

---

## Project Overview

A Boiling Liquid Expanding Vapour Explosion (BLEVE) can generate dangerous blast pressure effects. Predicting peak pressure is useful for risk assessment, safety analysis and hazard modelling.

This project uses structured tabular data to predict peak pressure values. Several machine learning models were developed and compared, with the final solution based on an ensemble approach combining strong-performing tree-based regression models.

---

## Objectives

- Clean and prepare structured BLEVE pressure data
- Explore relationships between input features and peak pressure
- Train and compare multiple regression models
- Improve prediction accuracy using target transformation and ensemble modelling
- Evaluate model performance using Mean Absolute Percentage Error (MAPE)
- Generate final predictions for the test dataset
- Apply explainability techniques to better understand model behaviour

---

## Dataset

The repository includes the following dataset and submission files:

```text
train.csv
test.csv
sample_prediction.csv
prediction.csv
```

The training dataset contains the target peak pressure values, while the test dataset contains unseen observations used for final prediction generation.

---

## Methods

The modelling workflow included:

- Exploratory data analysis
- Missing value checks
- Feature preparation
- Train-validation splitting
- Target transformation using PowerTransformer
- Model training and comparison
- Ensemble prediction
- Final test-set prediction generation
- Model interpretation using feature importance and partial dependence analysis

The main models considered included:

- Random Forest Regressor
- Gradient Boosting Regressor
- XGBoost Regressor
- LightGBM Regressor
- Weighted ensemble model

The final approach used a weighted ensemble of Gradient Boosting and LightGBM models with target transformation.

---

## Results

| Metric | Score |
|---|---:|
| Baseline Public MAPE | 0.252786 |
| Validation MAPE | 0.0997 |
| Public MAPE | 0.161348 |
| Private MAPE | 0.155453 |

The final ensemble improved substantially over the baseline and produced stable public and private leaderboard performance.

---

## Key Skills Demonstrated

- Python-based machine learning workflow
- Regression modelling
- Ensemble learning
- Feature engineering
- Target transformation
- Model evaluation using MAPE
- Explainable machine learning
- Reproducible notebook-based analysis
- Kaggle-style prediction file generation

---

## Repository Structure

```text
.
├── README.md
├── main.ipynb
├── requirements.txt
├── train.csv
├── test.csv
├── sample_prediction.csv
├── prediction.csv
└── .gitignore
```

---

## How to Run

Clone the repository:

```bash
git clone https://github.com/angadsingh-analyst/BLEVE-Peak-Pressure-Prediction-Using-Machine-Learning.git
cd BLEVE-Peak-Pressure-Prediction-Using-Machine-Learning
```

Install the required packages:

```bash
pip install -r requirements.txt
```

Open the notebook:

```bash
jupyter notebook main.ipynb
```

Run the notebook cells in order to reproduce the modelling workflow and generate predictions.

---

## Main Tools

- Python
- pandas
- NumPy
- scikit-learn
- XGBoost
- LightGBM
- Matplotlib
- Jupyter Notebook

---

## Data Availability

The dataset files are included in this repository with permission for portfolio and reproducibility purposes. The files are shared to demonstrate the machine learning workflow, model development process and final prediction pipeline.

These files should not be reused for academic submission or presented as someone else's coursework.

---

## Portfolio Note

This repository is a cleaned public portfolio version of a machine learning coursework project. Personal identifiers, academic declaration files and private submission documents have been removed.

The repository is shared to demonstrate applied skills in data preprocessing, regression modelling, ensemble learning, model evaluation and explainable AI.

---

## Author

Angad Singh  
Master of Predictive Analytics  
Perth, Western Australia
