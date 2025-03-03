# Sales forecasting
- The main goal is to predict sales of products in delivery app.
- Additionally, I researched effectiveness of gradient boosting models, SARIMA, LSTM
<div>
<img src="./data/picture.png" width="500"/>
</div>

## Introduction
- The predictions of products were made with classic ML models (CatBoost and LightGBM). 
- The predictions of number of clients were made with auto regression model (SARIMA) and LSTM.

## Data
Dataframe contained information about the date, weather conditions, product types, stores, and their locations. The history of the deliveries is available for previous 7 months.  

## Main results
- Compared effectiveness of two popular gradient boosting models (LightGBM and CatBoost).
    - Models demonstrated similar accuracy metrics of test dataframe. 
    - However, LightGBM was significantly faster to train and tune; and slightly more accurate
- Compared models for univariate time series. 
    - SARIMA outperformed LSTM in accuracy and training time.
    - LSTM was significantly less accurate (probably small data size) with WAPE=8 vs WAPE=4 in case of SARIMA.


