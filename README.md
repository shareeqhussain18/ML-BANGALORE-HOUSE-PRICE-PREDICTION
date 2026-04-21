# Bangalore Housing Price Prediction | End-to-End ML Pipeline with Streamlit Deployment

Live Demo:
https://bangalore-price-app-92izxhwhxbn8wc2uz422ya.streamlit.app

## Overview
Developed a regression-based machine learning system to predict residential property prices in Bangalore using structured housing data. The project implements a modular pipeline covering data preprocessing, model training, evaluation, and real-time inference.

## Key Contributions
- Built an end-to-end ML pipeline for reproducible training and inference
- Performed data cleaning (missing values, sqft normalization, outlier removal using price-per-sqft logic)
- Engineered features including one-hot encoding for high-cardinality location data
- Trained and compared multiple regression models using cross-validation
- Optimized model selection using GridSearchCV

## Model Performance
- Final Model: Linear Regression
- R² Score: 0.79
- MAE: 18
- RMSE: 45

## Deployment
- Deployed using Streamlit for interactive, real-time predictions
- End-to-end workflow: User Input → Preprocessing → Model Inference → Output

## Tech Stack
Python, Pandas, NumPy, Scikit-learn, Streamlit

## System Workflow
1. User inputs property details (sqft, BHK, bathrooms, location)
2. Input data is preprocessed using trained transformations
3. Model generates price prediction
4. Output displayed via web interface

## Project Structure
├── data/                # Raw and processed datasets  
├── notebooks/           # EDA and experimentation  
├── src/                 # Pipeline and model code  
├── models/              # Serialized model files  
├── app.py               # Streamlit application  
├── requirements.txt  
└── README.md  
