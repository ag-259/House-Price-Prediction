# House-Price-Prediction
This project implements an end-to-end machine learning pipeline for housing price prediction. It includes data preprocessing with imputation, scaling, and encoding, followed by training a Random Forest model. The pipeline supports both training and inference, saving models and generating predictions efficiently.

🏠 House Price Prediction System
📌 Overview

This project is a machine learning-based house price prediction system built using Scikit-learn. It predicts the median house value based on various housing features such as income, location, and other attributes.

The system follows a production-style pipeline, including:
  Data preprocessing
  Feature engineering
  Model training
  Model persistence
  Inference on new data
  
⚙️ Tech Stack
  Python
  Pandas, NumPy
  Scikit-learn
  Joblib (for model persistence)

🔄 Workflow

1. Data Preprocessing
  Missing values handled using median imputation
  Numerical features scaled using StandardScaler
  Categorical features encoded using OneHotEncoder
  Combined using ColumnTransformer

2. Feature Engineering
  Created an income category feature using binning
  Applied Stratified Sampling to maintain distribution

3. Model Training
  Model used: Random Forest Regressor
  Trained on processed dataset
  Pipeline ensures consistent preprocessing

4. Model Persistence
  Model saved as model.pkl
  Pipeline saved as pipeline.pkl
  Enables reuse without retraining

5. Inference
  Loads saved model and pipeline
  Transforms new input data
  Outputs predictions to output.csv


