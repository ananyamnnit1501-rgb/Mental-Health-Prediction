# 🧠 Mental Health Treatment Prediction System

An end-to-end Machine Learning project that predicts whether an individual is likely to require mental health treatment based on behavioral, demographic, and workplace-related factors. The project applies advanced ensemble learning techniques and compares multiple classification models to identify the best-performing approach.

---

##  Project Overview

Mental health disorders are becoming increasingly prevalent, making early identification and intervention crucial. This project leverages machine learning to analyze survey responses and predict treatment requirements using psychological, workplace, and demographic features.

The project covers the complete machine learning lifecycle, including data preprocessing, exploratory data analysis (EDA), feature engineering, model building, hyperparameter tuning, evaluation, and deployment preparation.



##  Dataset

- **Source:** Mental Health Survey Dataset
- **Rows:** 200,000+
- **Features:** Behavioral, workplace, demographic, and psychological attributes
- **Target Variable:** `treatment`



##  Project Workflow

```
Dataset
   │
   ▼
Data Cleaning
   │
   ▼
Exploratory Data Analysis (EDA)
   │
   ▼
Feature Engineering
   │
   ▼
Label Encoding
   │
   ▼
Train-Test Split
   │
   ▼
Model Training
   │
   ▼
Hyperparameter Tuning
   │
   ▼
Model Evaluation
   │
   ▼
Deployment Ready
```


##  Exploratory Data Analysis

Performed comprehensive EDA on a **200k+ row** dataset including:

- Dataset structure and data type analysis
- Missing value analysis and handling
- Duplicate record detection
- Gender and treatment distribution analysis
- Univariate analysis
- Bivariate analysis
- Multivariate analysis
- Correlation analysis
- Class balance verification
- Outlier investigation
- Psychological feature relationship analysis

### Key Insights

- Dataset contains approximately **82% male respondents**
- Target classes were nearly balanced
- Growing Stress and Mood Swings showed strong relationships with treatment requirements
- Psychological and workplace-related features were among the most influential predictors

---

##  Data Preprocessing

- Removed unnecessary and highly missing columns
- Handled missing values
- Label encoded categorical features
- Prepared ML-ready dataset
- Generated encoded dataset for model training

---

##  Machine Learning Models

The following classification models were implemented and compared:

- Random Forest Classifier
- XGBoost Classifier
- LightGBM Classifier
- Stacking Ensemble
  - Random Forest
  - XGBoost
  - LightGBM
  - Logistic Regression (Meta Learner)

---

##  Hyperparameter Tuning

Performed optimization using:

- GridSearchCV
- Stratified K-Fold Cross Validation

Optimized parameters such as:

- Number of estimators
- Tree depth
- Learning rate
- Minimum samples split
- Maximum features

---

##  Model Evaluation

Evaluation Metrics:

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC Score
- Confusion Matrix
- Cross Validation Score
- Overfitting Detection

### Best Model Performance

| Model | ROC-AUC |
|---------|---------|
| Random Forest | 0.787 |
| Tuned Random Forest | 0.823 |
| Stacking Ensemble | **0.877** |

---

## Visualizations

Generated visualizations including:

- Missing Value Analysis
- Feature Distribution
- Count Plots
- Correlation Heatmap
- ROC Curve
- Confusion Matrix
- Feature Importance
- Model Comparison

---

##  Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- LightGBM
- Matplotlib
- Seaborn
- Flask
- Joblib
- Google Colab

---

##  Project Structure

```
Mental-Health-Prediction/
│
├── Dataset/
│   ├── cleaned_dataset.csv
│   └── encoded_dataset.csv
│
├── notebooks/
│   ├── EDA.ipynb
│   ├── Model_Training.ipynb
│   └── Hyperparameter_Tuning.ipynb
│
├── models/
│   ├── random_forest.pkl
│   ├── tuned_random_forest.pkl
│   └── stacking_model.pkl
│
├── images/
│   ├── roc_curve.png
│   ├── confusion_matrix.png
│   ├── feature_importance.png
│   └── model_comparison.png
│
├── app.py
├── requirements.txt
└── README.md
```



##  Future Improvements

- SHAP Explainability
- CatBoost Implementation
- One-Hot Encoding Comparison
- Streamlit/Flask Web Deployment
- API Integration
- Cloud Deployment
