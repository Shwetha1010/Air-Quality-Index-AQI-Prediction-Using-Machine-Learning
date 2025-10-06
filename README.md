#  Air Quality Index (AQI) Prediction using Machine Learning

This project focuses on predicting the **Air Quality Index (AQI)** for Indian cities using various **machine learning regression models**.  
The goal is to analyze how different pollutants contribute to air quality and build a robust model that accurately forecasts AQI levels.

---

##  Project Overview

Air pollution is one of the major environmental challenges globally.  
This project leverages data-driven machine learning techniques to **predict AQI values** based on pollutants like PM2.5, NO₂, SO₂, CO, and O₃.

**Key Objectives:**
- Perform data cleaning, preprocessing, and feature engineering on multi-city AQI datasets.
- Visualize pollutant patterns and correlations to understand their effect on AQI.
- Train and compare multiple machine learning models to identify the most accurate predictor.

---

##  Dataset Description

The dataset consists of **daily and hourly air quality data** for multiple Indian cities.  
It includes the following key attributes:

| Feature | Description |
|----------|-------------|
| PM2.5, PM10 | Particulate Matter concentrations (µg/m³) |
| NO, NO₂, NOx | Nitrogen Oxides (µg/m³) |
| CO, SO₂, O₃ | Pollutant gases (mg/m³ or µg/m³) |
| NH₃ | Ammonia concentration |
| AQI | Air Quality Index (target variable) |
| City, Date | Metadata for analysis and visualization |

---

## Project Workflow

1. **Data Loading & Cleaning**  
   - Merged multi-city datasets (`city_day.csv`, `station_day.csv`, etc.)  
   - Handled missing values and removed irrelevant columns (`City`, `Date`, `AQI_Bucket`)

2. **Feature Engineering**  
   - Created new analytical features like **Average Pollutants per City** and **Average AQI per Year**  
   - Scaled and normalized numeric attributes for consistent modeling

3. **Data Visualization**  
   - Correlation heatmaps for pollutants vs AQI  
   - Line plots and time-series trends for yearly and city-wise AQI patterns  
   - Pollutant concentration distributions and seasonal variations

4. **Model Training & Evaluation**  
   - Implemented and compared multiple regression models:
     - Linear Regression  
     - Ridge & Lasso Regression  
     - Decision Tree Regressor  
     - Random Forest Regressor  
     - Gradient Boosting Regressor  
     - Support Vector Regressor (SVR)  
     - K-Nearest Neighbors (KNN)  
     - Multi-Layer Perceptron (MLP) Regressor  
   - Evaluated models using **Root Mean Squared Error (RMSE)** and **Accuracy**

---

## 📊 Model Performance

| Model | RMSE | Accuracy |
|--------|-------|-----------|
| Linear Regression | 53.29 | 0.7811 |
| Lasso Regression | 53.32 | 0.7811 |
| Ridge Regression | 53.29 | 0.7811 |
| Decision Tree Regressor | 63.40 | 0.9991 |
| **Random Forest Regressor** | **46.26** | **0.9812** |
| Gradient Boosting Regressor | 48.70 | 0.9059 |
| SVR | 61.61 | 0.8006 |
| KNN Regressor | 51.95 | 0.8910 |
| ElasticNet Regression | 53.47 | 0.7810 |
| MLP Regressor | 51.88 | 0.8783 |

🏆 **Best Model:** Random Forest Regressor  
📈 **Accuracy:** 98.12%  
📉 **RMSE:** 46.26

---

## 📚 Key Insights

- AQI strongly correlates with PM2.5, NO₂, and CO levels across urban areas.  
- Visualization of pollutant trends revealed distinct seasonal variations.  
- Random Forest outperformed other models, offering the best trade-off between accuracy and interpretability.

---

## 🚀 Results

✅ Achieved **98.12% accuracy** with **Random Forest Regressor**  
✅ Identified top pollutants influencing AQI  
✅ Delivered a scalable and explainable machine learning pipeline for air quality prediction

---



