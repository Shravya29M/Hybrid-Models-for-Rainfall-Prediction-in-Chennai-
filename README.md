
# Hybrid Models for Localized Rainfall Prediction in Chennai Using Statistical and Deep Learning Approaches

## Project Overview

This project involves forecasting rainfall data for the city of Chennai using several time-series forecasting models: N-BEATS, Prophet, Exponential Smoothing, and a Hybrid model. The goal is to predict the future rainfall trends and evaluate the performance of different models on historical rainfall data.

The dataset used in this project contains total annual rainfall data for Chennai, spanning several years, with a focus on data from 2000 onwards.

## Models Implemented

### 1. **Data Preprocessing and EDA**
   - Loaded and filtered the dataset from 2000 onwards.
   - Performed exploratory data analysis (EDA) to visualize the total annual rainfall trends and monthly rainfall patterns.

### 2. **N-BEATS Model**
   - Implemented a Neural Network model based on N-BEATS for forecasting rainfall using historical data.
   - Preprocessed the data into sequences for training the model.
   - Evaluated the model using Root Mean Squared Error (RMSE).
   - Visualized the actual vs. predicted rainfall data.

### 3. **Prophet Model**
   - Used Facebook Prophet for time-series forecasting.
   - Prepared the dataset for Prophet by renaming columns and converting the year to a datetime format.
   - Forecasted future rainfall values and compared them with actual values.
   - Visualized forecasted vs actual rainfall trends and components.

### 4. **Exponential Smoothing (Holt-Winters)**
   - Applied Exponential Smoothing for forecasting rainfall trends.
   - Used an additive trend component for the model.
   - Evaluated the model using RMSE and visualized the actual, fitted, and forecasted values.

### 5. **Hybrid Model**
   - Combined the power of the N-BEATS and Prophet models to create a hybrid model.
   - Integrated the strengths of both models to improve forecasting accuracy.
   - Evaluated and compared the performance of the hybrid model with other individual models.

## Requirements

You will need the following Python libraries to run the project:

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- keras
- xgboost
- statsmodels
- torch
- prophet
- neuralforecast

Install them using the following command:

```bash
pip install pandas numpy matplotlib scikit-learn keras xgboost statsmodels torch prophet neuralforecast
```

## Dataset

The dataset used in this project contains the following columns:

- `Year`: The year of the recorded rainfall.
- `Total`: The total rainfall recorded for the respective year.

The data has been filtered to focus on rainfall data from the year 2000 onwards.

## Results

- **N-BEATS RMSE**: 70.92
- **Prophet RMSE**: To be calculated based on forecast vs actual comparison.
- **Exponential Smoothing RMSE**: To be calculated based on fitted vs actual data.
  
For each model, actual vs predicted rainfall plots are displayed to assess performance visually.

## Usage

1. **Data Preprocessing & Visualization**: 
   - Load the dataset and filter it from 2000 onwards.
   - Visualize the total annual rainfall trends and monthly rainfall patterns.

2. **Modeling**: 
   - Choose the forecasting model (N-BEATS, Prophet, Exponential Smoothing, or Hybrid).
   - Train the model using the historical data and generate predictions for future rainfall.

3. **Evaluation**: 
   - Calculate the RMSE for model evaluation.
   - Compare the forecasted values with the actual values to determine model accuracy.

4. **Visualization**: 
   - Plot actual vs predicted rainfall values for better understanding.

## Conclusion

This project demonstrates the use of multiple time-series forecasting models to predict future rainfall data for Chennai. The comparison of different models, such as N-BEATS, Prophet, Exponential Smoothing, and a Hybrid model, provides valuable insights into their accuracy and effectiveness for this type of forecasting task.

Feel free to explore the different models and tweak the code as needed to improve the performance further.

