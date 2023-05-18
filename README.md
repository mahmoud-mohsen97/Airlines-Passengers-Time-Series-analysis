# Airlines-Passengers-Time-Series-analysis

The airline industry relies heavily on forecasting passenger demand to optimize operational efficiency and profitability. However, accurately predicting passenger demand is a complex task due to various external and internal factors, such as seasonality, economic conditions, and marketing campaigns.
<p align="center">
    <img src="https://user-images.githubusercontent.com/43541909/233919681-d5617d2e-0bca-4ca4-a6de-a9abd1046948.png" alt="Image Description">
</p>

- In this project, we aim to develop a time series forecasting model using historical airline passenger data to accurately predict future passenger demand.
- The model should take into account different patterns and trends in the data, such as seasonality and trend, and incorporate external factors that affect passenger demand. 
- The goal is to provide actionable insights to airline companies to make informed decisions on capacity planning, pricing, and marketing strategies.


## Walk Through The Project
* Exploratory data analysis will be conducted to analyze the time series data using visual plots and comment on the findings.

* The following forecasting approaches will be applied and compared:
    * Simple Moving Average
    * Naïve Forecasting
    * Weight Moving Average
    * Simple Linear Regression Model
    * Classical Decomposition Approach
    * STL Decomposition Approach
    * ARIMA/S-ARIMA Model
    * Exponential Smoothing
    * Facebook Prophet Algorithm
    * Supervised Machine Learning algorithm (XGBOOST Regressor)
    
* Each approach will be commented on to explain why the results are produced in that manner and their pros and cons.

* Before applying any approach, stationarity of the time series data will be checked and necessary transformations will be applied.

* The classical and STL decomposition approaches will be compared based on the decomposed components.

* Different ARIMA models will be tested based on ACF, PACF plots, summary statistics, and residuals analysis, and the AIC or BIC will also be checked.

* For exponential smoothing, single, double, and triple exponential smoothing approaches will be applied, and the need for dampening will be determined both theoretically and practically.

* The Facebook Prophet algorithm will be applied, and its effectiveness will be assessed.

* Finally, a supervised machine learning algorithm (XGBOOST Regressor) will be applied using lag features (Yt−1, Yt−2, ... , avg(yt−n)).



## Evaluation Metric
#### The dataset will be evaluated using the RMSE metric

<p align="center">
    <img src="https://user-images.githubusercontent.com/43541909/233920019-19c77893-6a44-4cb8-9d18-6cf7944d7018.png" alt="Image Description">
</p>



#### Through three different spliting techniques:

* roll-forward

<p align="center">
    <img src="https://user-images.githubusercontent.com/43541909/233920373-dc886d32-5af5-4163-8652-b613d113f197.png" alt="Image Description">
</p>



* simple train-test split

<p align="center">
    <img src="https://user-images.githubusercontent.com/43541909/233920199-25e36a12-f747-4449-bb78-5fc3598cbd21.png" alt="Image Description">
</p>



* Time series cross-validation from sklearn

<p align="center">
    <img src="https://user-images.githubusercontent.com/43541909/233920288-c70cc4e9-5ec1-40ec-b5cc-434cd901b2fb.png" alt="Image Description">
</p>

## Results
| Technique                                | Best RMSE|
|------------------------------------------|-------|
| Simple Moving Average                    | 112.16|
| Naïve forecast                           | 105.75|
| Weighted Moving Average                  | 122.87|
| Linear Regression Model                  | 85.7  |
| Classical Decomposition                  | 60    | 
| STL Decomposition                        | 68.7  |
| ARIMA                                    | 39.72 |
| S-ARIMA                                  | 13.76 |
| Exponential Smoothing Single             | 47.36 |
| Exponential Smoothing Double Additive    | 47.34 |
| Exponential Smoothing Double Multiplicative| 43.7|
| Exponential Smoothing Triple Additive    | 12.3 |
| Exponential Smoothing Triple Multiplicative |**11.51**|
| FB Prophet                               |22.48|
| XGBOOST Regressor                        |49.6|

## Conclusion
we have analyzed the airline passengers dataset using various time series techniques and found that the **Exponential Smothing Triple Multiplicative model** with **RMSE =11.51**  which is the best results overall when predicting future passenger numbers. 
