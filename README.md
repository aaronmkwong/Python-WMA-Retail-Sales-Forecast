# Python-WMA-Retail-Sales-Forecast


**Purpose & Summary**

The program evaluates a weighted moving average (WMA) method to forecast Western Canada (BC, AB, SK, MB) retail sales for the period 2017 to 2019. Mean absolute percentage error (MAPE) is used to evaluate all forecast scenario combinations of 2, 3, 4, 5 and 6 month moving averages and 0.1 incremented weightings, e.g. 3 month moving average with weights of 0.1, 0.2 and 0. 7. Before WMA is used to forecast, sales are deasonalized using the ratio-to-moving-average method and a seasonality factor is determined. The seasonality factor is then applied to the deseasonalized sales forecast values to arrive at the final sales forecast values.

**Results & Visualizations**

comments to be entered here

![alt text](https://github.com/aaronmkwong/Python-WMA-Retail-Sales-Forecast/blob/main/Images/01_Western_Canada_Retail_Sales.JPG)

comments to be entered here

![alt text](https://github.com/aaronmkwong/Python-WMA-Retail-Sales-Forecast/blob/main/Images/02_Seasonality_Factors.JPG)

comments to be entered here

![alt text](https://github.com/aaronmkwong/Python-WMA-Retail-Sales-Forecast/blob/main/Images/03_Deasonalized_Sales.JPG)

comments to be entered here

![alt text](https://github.com/aaronmkwong/Python-WMA-Retail-Sales-Forecast/blob/main/Images/04_Summary_Statistics_Forecast.JPG)

comments to be entered here

![alt text](https://github.com/aaronmkwong/Python-WMA-Retail-Sales-Forecast/blob/main/Images/05_Error_Distribution.JPG)

comments to be entered here

![alt text](https://github.com/aaronmkwong/Python-WMA-Retail-Sales-Forecast/blob/main/Images/06_Actual_Forecast_MAPE.JPG)

comments to be entered here

**Data Sources**

Statistics Canada via the Web Data Service (API database access) using the vector IDs specific for clothes and hobby retail sales for the provinces of BC, AB, SK and MB. 
https://www.statcan.gc.ca/eng/developers/wds
