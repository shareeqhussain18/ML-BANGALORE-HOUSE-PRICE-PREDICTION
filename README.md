# ML-HOUSE-PRICE-END-TO-END

END-TO-END MACHINE LEARNING PROJECT FOR BANGALORE HOUSE PRICE PREDICTION WITH MODULAR PIPELINE, MODEL COMPARISON, AND STREAMLIT DEPLOYMENT.
---

## 🚀 LIVE DEMO
👉  https://bangalore-price-app-92izxhwhxbn8wc2uz422ya.streamlit.app

---
## 🧩 PROBLEM STATEMENT

The goal of this project is to predict house prices in Bangalore based on key features such as:

- Total square feet
- Number of bedrooms (BHK)
- Number of bathrooms
- Location
---

## 🧹 DATA ANALYSIS & CLEANING

- Removed null and inconsistent values
- Standardized sqft feature (handled ranges like 1000–1200)
- Filtered unrealistic entries using domain logic
- Reduced dimensionality by grouping rare locations
- Outlier removal based on price per sqft
---
 
 ## ⚙️ FEATURE ENGINEERING

- Converted categorical location data using one-hot encoding
- Normalized and cleaned numerical features
- Created meaningful features for better model performance

---

## 🤖 MODEL BUILDING

Trained multiple regression models:

- Linear Regression
- Ridge Regression
- Lasso Regression

Used cross-validation to ensure stability and avoid overfitting.

---

## 📊 MODEL EVALUATION

| Model             |  R² Score |
|-------------------|-----------|
| Linear Regression |  0.83     |
| Lasso Regression  |  0.78     |
| Decision Tree     |  0.75     |

**Final Model Selected:** Linear Regression (best performance based on GridSearchCV with cross-validation)

Model achieved R² ≈ 0.79 with MAE ≈ 18 (~19% of mean price) and RMSE ≈ 45 (~46% of mean), demonstrating reasonable predictive performance on unseen data.  

### Model Selection Reasoning  ###

GridSearchCV was used to tune hyperparameters and evaluate models using cross-validation. Linear Regression achieved the highest R² score and demonstrated better generalization compared to other models.
---

---

## 🧠 ML PIPELINE

1. Data Cleaning
2. Feature Engineering
3. Model Training
4. Cross-validation
5. Model Selection
6. Model Serialization (pickle)
7. Deployment

---

##### 🌐 WEB APPLICATION   ####

A Streamlit-based web application is built to make predictions in real-time.

### System workFlow:
User Input → Streamlit UI → Data Preprocessing → Model → Prediction Output


## 🏗️ System Architecture

The system follows a modular prediction pipeline:

1. **User Interface (Streamlit)**
   - Accepts user inputs (sqft, BHK, bathrooms, location)

2. **Data Preprocessing Layer**
   - Handles feature transformation
   - Encodes categorical variables (location)
   - Applies same transformations used during training

3. **Model Inference Layer**
   - Loads the trained regression model (pickle file)
   - Generates predictions based on processed input

4. **Output Layer**
   - Displays predicted house price in real-time


### Features:
- User-friendly interface
- Takes input: sqft, BHK, bathrooms, location
- Instant price prediction
- Lightweight and fast

---

## 🛠️ TECH STACK

- Python
- Pandas
- NumPy
- Scikit-learn
- Streamlit
---

## 🚀 LIVE DEMO
👉  https://bangalore-price-app-92izxhwhxbn8wc2uz422ya.streamlit.app


## 📂 PROJECT STRUCTURE
