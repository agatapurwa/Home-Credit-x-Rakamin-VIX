# Home-Credit-x-Rakamin-VIX: Home Credit Default Risk Prediction 📊

An end-to-end Machine Learning project to predict the probability of clients defaulting on their loans. This project is developed as part of the Data Science Virtual Internship Experience (VIX) with Rakamin Academy and Home Credit Indonesia.

## 🎯 Project Objective
Financial institutions face significant risks when lending to clients with insufficient or non-existent credit histories. The goal of this project is to build a robust machine learning model that leverages alternative data (telco, transactional, etc.) to accurately predict clients' repayment abilities, ensuring that capable clients are not rejected while minimizing default risks.

## 🛠️ Technical Workflow & Highlights

### 1. Data Cleansing & Anomaly Handling
- **Edge Case Mitigation:** Successfully identified and handled the `365243` anomaly in the `DAYS_EMPLOYED` feature, treating it as a distinct category/NaN to prevent extreme skewness in the dataset.
- **Feature Engineering:** Extracted and transformed time-based features (converting days to absolute years) and merged relational tables (bureau data, previous applications) to enrich the primary dataset.

### 2. Enterprise-Grade Preprocessing Pipeline
Built a scalable and reproducible data transformation pipeline utilizing Scikit-Learn's `ColumnTransformer`:
- **Categorical Features:** Applied `SimpleImputer` (most frequent) followed by `OneHotEncoder`.
- **Numerical Features:** Applied `SimpleImputer` (median) followed by `StandardScaler` to ensure optimal gradient convergence.

### 3. Machine Learning Modeling
Developed and evaluated predictive models using the preprocessed pipeline:
- **Logistic Regression:** Used as an interpretable baseline model.
- **Random Forest Classifier:** Utilized for capturing non-linear relationships and extracting feature importance.

## 📂 Repository Structure
* `Home_Credit_Scorecard_Model.ipynb` : The primary Jupyter Notebook containing EDA, custom preprocessing pipeline, feature engineering, and model training.
* `gambar/` : Directory containing architectural diagrams and visualization outputs.
* `Dataset/` : Ignored via `.gitignore` in compliance with data privacy policies and repository size limits.

## 🚀 Reproduction & Data Notice
> **Note on Dataset:** The dataset used in this project was provided as part of the Rakamin Virtual Internship Experience (VIX) and contains specific feature structures/column mappings tailored to the program. 
> 
> Due to data distribution policies and structural differences from the original raw Kaggle dataset, the raw data files are kept private. This repository serves as a demonstration of data science workflows, feature engineering logic, and machine learning pipeline architecture.
