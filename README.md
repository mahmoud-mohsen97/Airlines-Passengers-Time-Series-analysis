# Airlines-Passengers-Time-Series-analysis

The airline industry relies heavily on forecasting passenger demand to optimize operational efficiency and profitability. However, accurately predicting passenger demand is a complex task due to various external and internal factors, such as seasonality, economic conditions, and marketing campaigns. In this project, we aim to develop a time series forecasting model using historical airline passenger data to accurately predict future passenger demand. The model should take into account different patterns and trends in the data, such as seasonality and trend, and incorporate external factors that affect passenger demand. The goal is to provide actionable insights to airline companies to make informed decisions on capacity planning, pricing, and marketing strategies.

![image](https://user-images.githubusercontent.com/43541909/233919681-d5617d2e-0bca-4ca4-a6de-a9abd1046948.png)


1. The dataset will be evaluated using the**RMSE metric** 


![image](https://user-images.githubusercontent.com/43541909/233920019-19c77893-6a44-4cb8-9d18-6cf7944d7018.png)


and **three** different evaluation techniques:

**roll-forward**,


![image](https://user-images.githubusercontent.com/43541909/233920373-dc886d32-5af5-4163-8652-b613d113f197.png)


**simple train-test split**,


![image](https://user-images.githubusercontent.com/43541909/233920199-25e36a12-f747-4449-bb78-5fc3598cbd21.png)


and time series **cross-validation** from sklearn.


![image](https://user-images.githubusercontent.com/43541909/233920288-c70cc4e9-5ec1-40ec-b5cc-434cd901b2fb.png)


2. Exploratory data analysis will be conducted to analyze the time series data using visual plots and comment on the findings.

3. The following forecasting approaches will be applied and compared:
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
    
4. Each approach will be commented on to explain why the results are produced in that manner and their pros and cons.

5. Before applying any approach, stationarity of the time series data will be checked and necessary transformations will be applied.

6. The classical and STL decomposition approaches will be compared based on the decomposed components.

7. Different ARIMA models will be tested based on ACF, PACF plots, summary statistics, and residuals analysis, and the AIC or BIC will also be checked.
For exponential smoothing, single, double, and triple exponential smoothing approaches will be applied, and the need for dampening will be determined both theoretically and practically.

8. The Facebook Prophet algorithm will be applied, and its effectiveness will be assessed.

9. Finally, a supervised machine learning algorithm (XGBOOST Regressor) will be applied using lag features (Yt−1, Yt−2, ... , avg(yt−n)).

In summary, the project involves forecasting air passenger traffic using various time series forecasting techniques and comparing their effectiveness. The project will also include exploratory data 
