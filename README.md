**Credit Card Fraud Detection**
A data preprocessing and machine learning pipeline for detecting fraudulent credit card transactions using the Kaggle Credit Card Fraud Dataset (285807 transactions, 31 features).

**Overview**
Credit card fraud is a highly imbalanced classification problem — only 0.17% of transactions in this dataset are fraudulent. This project focuses on building a robust preprocessing pipeline that handles class imbalance and prepares data for downstream model training.

**What I Did**
- Data Cleaning — Identified and removed 1,081 duplicate records, reducing the dataset from 284,807 to 283,726 transactions
- Missing Value Check — Validated data completeness across all 31 features
- Feature Engineering - Extracted hour-based features from the Time column to capture temporal fraud patterns
- Scaling — Applied RobustScaler to normalise features, chosen for its resistance to outliers common in fraud data
- Class Imbalance Handling — Implemented both SMOTE (oversampling) and Random Undersampling to address the extreme class imbalance (99.83% legitimate vs 0.17% fraud)
-  Stratified Splitting— Used stratified train/test splits to preserve class distribution across training and evaluation sets

**Tech Stack**
- Python
- pandas, NumPy
- scikit-learn (RobustScaler, train_test_split)
- imbalanced-learn (SMOTE)

**Dataset**
The dataset contains credit card transactions made by European cardholders over two days in September 2013. Features V1–V28 are PCA-transformed for confidentiality. Only Time and Amount are original features.
**Total transactions:** 284,807
**Fraudulent**: 492 (0.17%)
**Features**: 31 (28 PCA components + Time, Amount, Class)

Author
Bolortulga Seded - MSc Big Data and Data Science, Northumbria University London
