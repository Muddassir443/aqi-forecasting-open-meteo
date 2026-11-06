# AQI Prediction using Random Forest

## Overview
This project predicts the US Air Quality Index (AQI) from hourly pollutant 
measurements using a Random Forest Regressor. Data is collected directly from 
the Open-Meteo Air Quality API for the Vijayawada region (Jan 2026 to Nov 2026).

## Data
- **Source:** Open-Meteo Air Quality API (no API key required)
- **Frequency:** Hourly
- **Features:** PM10, PM2.5, carbon monoxide, nitrogen dioxide, sulphur dioxide, 
  ozone, dust, plus date-based features
- **Target:** US AQI

## Approach
1. Fetched hourly data from the API and saved it as a CSV
2. Cleaned the data and extracted date features
3. Split into training and test sets
4. Trained a Random Forest Regressor
5. Evaluated with R² and visualized actual vs. predicted values
6. Saved the trained model with pickle

## Results
- Training R²: XX
- Test R²: XX

## Tech Stack
Python, pandas, NumPy, scikit-learn, matplotlib, requests

## How to Run
1. Clone the repo
2. Install dependencies: `pip install -r requirements.txt`
3. Open the notebook and run all cells

## Future Improvements
- Forecast future AQI from past readings (time-series approach) instead of 
  predicting the current value
- Use a time-based train/test split to avoid data leakage
- Add lag features and hyperparameter tuning
- Compare with other models such as XGBoost
