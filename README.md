Air Quality Prediction and Forecasting
📌 Overview
This project focuses on analyzing and forecasting Air Quality Index (AQI) levels using historical pollution data and machine learning techniques. By leveraging time-series preprocessing and feature engineering, this end-to-end Python pipeline transforms raw environmental sensor data into actionable predictive signals.
🚀 Key Features
Time-Series Preprocessing: Handled missing sensor data, temporal sorting, and date-time conversions to maintain strict chronological integrity.
Feature Engineering: Implemented time-series lag features (historical rolling windows) and feature scaling to prepare pollutant data (CO, NO2, PM2.5, etc.) for modeling.
Machine Learning Pipeline: Built a robust predictive model using RandomForestRegressor (with the data architecture easily adaptable for time-series forecasting tools like Prophet).
Strict Temporal Validation: Split training and testing sets chronologically (walk-forward validation) to completely prevent data leakage and ensure real-world viability.
Data Visualization: Generated clear, professional comparisons of historical actuals versus model predictions.
🛠️ Tech Stack
Data Manipulation & Analysis: pandas, numpy
Machine Learning: scikit-learn
Data Visualization: matplotlib, seaborn
📊 Model Performance
The final Random Forest Regressor demonstrated excellent predictive capabilities on the testing set, rarely deviating from the actual Air Quality Index category:
R-squared (R2): 0.848 (Successfully captured ~85% of the variance in air quality)
Mean Absolute Error (MAE): 0.177
Root Mean Squared Error (RMSE): 0.232

<img width="830" height="412" alt="Screenshot 2026-06-21 202640" src="https://github.com/user-attachments/assets/4ccf05dc-0041-48b0-b918-559f54d6da83" />
