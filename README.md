# Heart Disease ML Assignment

This project implements multiple machine learning classification models to predict heart disease.  
It includes both Jupyter notebooks for training and a Streamlit app for deployment.

## Repository Structure
- `app.py` → Streamlit app for predictions and evaluation
- `requirements.txt` → Dependencies for running the app
- `model/` → Contains trained models (`.pkl`) and notebooks (`.ipynb`)
- `README.md` → Project documentation

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/2025aa05167-shriyansh/heart-disease-ml-assignment-.git
 Problem Statement
Heart disease is one of the leading causes of mortality worldwide, and early detection is critical for effective treatment and prevention. The goal of this project is to develop machine learning models that can predict the likelihood of heart disease based on patient health attributes. By analyzing clinical and demographic features such as age, sex, chest pain type, blood pressure, cholesterol levels, and other medical indicators, the models aim to assist healthcare professionals in identifying high‑risk patients quickly and accurately.
This assignment demonstrates how different machine learning algorithms perform on the same dataset, comparing their predictive accuracy and reliability.

Dataset Description
The dataset used in this project is the Heart Disease dataset (commonly derived from the Cleveland Heart Disease dataset). It contains patient records with multiple attributes that are clinically relevant for diagnosing heart disease.
Features:
- Age: Patient’s age in years
- Sex: Gender (1 = male, 0 = female)
- cp: Chest pain type (categorical)
- trestbps: Resting blood pressure (mm Hg)
- chol: Serum cholesterol (mg/dl)
- fbs: Fasting blood sugar (> 120 mg/dl)
- restecg: Resting electrocardiographic results
- thalach: Maximum heart rate achieved
- exang: Exercise‑induced angina
- oldpeak: ST depression induced by exercise relative to rest
- slope: Slope of the peak exercise ST segment
- ca: Number of major vessels colored by fluoroscopy
- thal: Thalassemia (categorical)
- target: Diagnosis of heart disease (1 = disease present, 0 = no disease)
  
ML Model Name:
Logistic Regression
Decision Tree
KNN
Naive Bayes
Random Forest
XGBoost
   
#Models Used & Evaluation

#Comparison Table

| ML Model Name       | Accuracy | AUC   | Precision | Recall | F1    | MCC   |
|---------------------|----------|-------|-----------|--------|-------|-------|
| Logistic Regression | 0.868    | 0.944 | 0.848     | 0.905  | 0.876 | 0.738 |
| Decision Tree       | 1.000    | 1.000 | 1.000     | 1.000  | 1.000 | 1.000 |
| KNN                 | 0.824    | 0.949 | 0.848     | 0.800  | 0.824 | 0.650 |
| Naive Bayes         | 0.824    | 0.883 | 0.829     | 0.829  | 0.829 | 0.649 |
| Random Forest       | 1.000    | 1.000 | 1.000     | 1.000  | 1.000 | 1.000 |
| XGBoost             | 1.000    | 1.000 | 1.000     | 1.000  | 1.000 | 1.000 |

#Observations

| ML Model Name             | Observation about model performance                                                                 |
|----------------------------|-----------------------------------------------------------------------------------------------------|
| Logistic Regression        | Strong baseline model with high accuracy and balanced precision/recall. Performs well but not perfect. |
| Decision Tree              | Achieved perfect scores, but may be overfitting to the dataset.                                     |
| KNN                        | Moderate performance, recall slightly lower than precision, indicating sensitivity to neighborhood size. |
| Naive Bayes                | Balanced precision and recall, but overall accuracy lower compared to ensemble methods.             |
| Random Forest (Ensemble)   | Perfect scores across all metrics, robust ensemble method, likely generalizes well.                 |
| XGBoost (Ensemble)         | Perfect scores, powerful ensemble boosting method, strong predictive performance.                   |
