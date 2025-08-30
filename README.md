# Disease Diagnosis Using Symptoms

This repository contains the implementation of a machine learning pipeline designed to predict common diseases based on patient-reported symptoms. The project was developed as part of a data hackathon challenge with the goal of leveraging AI to assist in rapid, symptom-based diagnosis.

# Project Overview

Accurate disease diagnosis is often hindered by overlapping symptoms and imbalanced representation of certain illnesses. This work explores the use of supervised learning models to classify diseases from tabular symptom data, where each row represents a patient case and each column corresponds to a binary symptom indicator.

# Methodology

The workflow follows a structured, experiment-driven approach:

Data Preprocessing; Cleaned, encoded, and balanced the dataset for model training while preserving class diversity.

Baseline Models; Trained Decision Tree, Random Forest, XGBoost, and LightGBM with class-weight balancing to establish benchmarks.

Hyperparameter Tuning; Applied RandomizedSearchCV to optimize each model’s parameters, leading to significant performance improvements.

Ensemble Learning; Constructed a soft voting ensemble of the three best-performing tuned models, achieving superior predictive accuracy and robustness.

# Results

Baseline models achieved strong performance, with Random Forest, XGBoost, and LightGBM performing best.

Hyperparameter tuning further improved accuracy and F1 scores across most classes.

The ensemble model demonstrated the highest overall reliability, effectively leveraging the strengths of individual learners.

# Significance

This project demonstrates the viability of AI-powered decision support in healthcare, especially in settings where access to diagnostic tools is limited. By relying solely on symptom data, the models provide a scalable and cost-effective solution to support frontline health workers and clinicians.

# Future Work

To further enhance diagnostic precision, the next steps include:

Incorporating demographic and clinical variables (e.g., age, gender, BMI).

Exploring deep learning and neural ensemble methods.

Deploying the solution as an interactive web or mobile application.
