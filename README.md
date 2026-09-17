# Heart Risk Predictor

An end to end machine learning project that predicts the 10 year risk of 
coronary heart disease (CHD) using the Framingham Heart Study dataset.  

## Business Question
Can we use a patient's health data to predict their 10-year heart disease 
risk, so doctors can act early?

## Dataset
Framingham Heart Study 4240 rows, 16 columns, target: TenYearCHD (imbalanced, 
approx. 15% at risk).  
Source: https://www.kaggle.com/datasets/aasheesh200/framingham-heart-study-dataset

## Steps
- EDA (missing values, imbalance check)
- Preprocessing (train/test split, median imputation, StandardScaler)
- Model training & tuning (Logistic Regression, LinearSVC, Random Forest with GridSearchCV, F1 scoring)
- Model evaluation
- Unsupervised learning (K-Means and PCA)
- Feature importance

## Result
Final model: **Logistic Regression** — ROC-AUC 0.71, Recall 0.63 for at-risk 
patients. The most important risk factors were age, smoking, and blood pressure.

## Tools
Python, pandas, scikit-learn, matplotlib, seaborn

## How to run
Open `heart_risk_predictor.ipynb` in Jupyter and run all cells.
