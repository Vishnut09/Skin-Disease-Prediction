# Skin-Disease-Prediction

Skin Disorder Prediction using Machine Learning

#Project Overview

This project focuses on building a machine learning–based decision support system to classify six types of erythemato-squamous skin disorders using clinical and histopathological features.

Skin diseases often share similar visible symptoms, making accurate diagnosis difficult without invasive procedures like biopsy. This project aims to assist dermatologists by providing a reliable, interpretable, and data-driven predictive model for early screening and disease classification.

# Objective

To develop a multi-class classification model that predicts the type of skin disorder based on:

Clinical attributes (symptom observations)

Histopathological attributes (microscopic tissue analysis)

Patient age

Family history

The final model serves as a clinical decision-support tool, not a replacement for medical diagnosis.

📊 Dataset Description

The dataset contains:

34 Features

12 Clinical attributes

22 Histopathological attributes

1 Age feature

1 Target class (Skin Disease Type)

Feature Characteristics:

Most features are ordinal values (0–3) representing severity

Family history is binary (0 or 1)

Target variable contains 6 disease classes

# Exploratory Data Analysis (EDA)

Key analysis steps performed:

Checked class distribution (multi-class classification)

Analyzed feature distributions and severity patterns

Studied correlation between histopathological features

Identified high-impact features such as:

Parakeratosis

Hyperkeratosis

Acanthosis

Munro microabscess

EDA confirmed that histopathological features provide strong discriminative power.

# Data Preprocessing

Median imputation for missing values

Feature scaling using StandardScaler

Label encoding of target variable

Stratified train-test split to maintain class balance

Pipeline implementation for reproducibility

# Machine Learning Models Used

The following models were trained and evaluated:

Logistic Regression

Decision Tree

Support Vector Machine (SVM)

Random Forest

XGBoost

📈 Evaluation Metrics:

Accuracy

Precision

Recall

Macro F1 Score (primary metric)

🏆 Best Performing Model

Ensemble models such as Random Forest and XGBoost performed the best due to:

Ability to capture non-linear feature interactions

Robustness to noise

Better handling of overlapping disease characteristics

Strong multi-class performance

🔬 Model Interpretability

To ensure clinical trust:

Feature importance analysis was performed

Permutation importance was evaluated

Predictions were analyzed using confusion matrix

Interpretability was prioritized due to healthcare domain requirements.

# Challenges Faced

Overlapping symptoms across diseases

Handling ordinal medical features correctly

Ensuring balanced multi-class evaluation

Maintaining interpretability while improving accuracy

These challenges were addressed using ensemble methods, cross-validation, and macro-level metrics.

# Future Improvements

Add SHAP-based explainability

Probability calibration for clinical confidence scoring

External dataset validation

Extend to image-based deep learning models (CNNs)

Deploy as a web-based clinical support system

# Tech Stack

Python

Pandas

NumPy

Scikit-learn

XGBoost

Matplotlib

Seaborn

📂 Project Structure
Skin-Disorder-Prediction/
│
├── skin_disorder_prediction.ipynb
├── README.md
├── requirements.txt
└── dataset.csv

🧠 Key Learnings

Handling structured medical data

Multi-class classification evaluation

Importance of macro F1 score in healthcare

Model interpretability in sensitive domains

Building reproducible ML pipelines

⚠️ Disclaimer

This model is intended for educational and research purposes only.
It should be used as a decision-support tool and not as a replacement for professional medical diagnosis.
