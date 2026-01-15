# Energy-Production
End-to-end exploratory analysis, machine learning, clustering, and time-series forecasting

# Energy Production Analysis and Forecasting

This project performs a multi-faceted machine learning analysis on a multi-year energy production dataset. It aims to understand production patterns across different sources (Wind and Solar) and build predictive models for future energy output.

## 📊 Dataset Overview
The dataset contains 50,000+ records of energy production, including:
- **Temporal Features:** Date, Start/End Hour, Day of Year, Season.
- **Categorical Features:** Energy Source (Wind, Solar, Mixed), Month, Day Name.
- **Target:** Production (Numerical).

## 🚀 Implemented Algorithms

### 1. Exploratory Data Analysis (EDA)
- Analyzed production trends across seasons and months.
- Visualized the hourly cycle of Solar vs. Wind energy.

### 2. Regression (Random Forest)
- **Model:** Random Forest Regressor.
- **Goal:** Predict hourly production levels.
- **Key Features:** Day of Year and Start Hour were identified as the most significant predictors.


### 3. Clustering (Unsupervised Learning)
- **K-Means:** Grouped production data into 3 distinct clusters (Low-production, Peak Solar, and High Wind).
- **DBSCAN:** Used for anomaly detection to identify production outliers and noise.

### 4. Time Series Forecasting
- **Moving Averages:** 7-day and 30-day trends.
- **Deep Learning:** LSTM (Long Short-Term Memory) architecture for sequential daily forecasting.
- **Evaluation:** Performance measured using MAE, MSE, RMSE, and MedAE.

## 📈 Results
- The Random Forest model explains ~52% of the variance in production.
- KNN classification successfully distinguishes Solar from Wind with high precision.
- Time series analysis reveals strong seasonal patterns, particularly higher solar output in Summer months.
