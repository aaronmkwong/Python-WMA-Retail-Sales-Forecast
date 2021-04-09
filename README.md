# Python-WMA-Retail-Sales-Forecast


**Purpose**

The program evaluates a weighted moving average (WMA) method to forecast Western Canada (BC, AB, SK, MB) retail sales for the period 2017 to 2019 by month. Mean absolute percentage error (MAPE) is used to evaluate all forecast scenario combinations of 2, 3, 4, 5 and 6 month moving averages and 0.1 incremented weightings, e.g. 3 month moving average with weights of 0.1, 0.2 and 0. 7. Before WMA is used to forecast, sales are deseasonalized using the ratio-to-moving-average method and a seasonality factor is determined. The seasonality factor is then applied to the deseasonalized sales forecast values to arrive at the final sales forecast values.

**Results**

A line graph of actual retail sales by category (only clothes and hobby used for this evaluation) shows a consistent seasonal pattern across all provinces.  

![alt text](https://github.com/aaronmkwong/Python-WMA-Retail-Sales-Forecast/blob/main/Images/01_Western_Canada_Retail_Sales.JPG)

The seasonality factors are displayed in a data frame with a colour gradient to highlight the monthly variation in sales, consistent with significant winter holiday shopping.   

![alt text](https://github.com/aaronmkwong/Python-WMA-Retail-Sales-Forecast/blob/main/Images/02_Seasonality_Factors.JPG)

A line graph of deseasonalized actual retail sales shows the remaining trend and cycle components of the time series.  

![alt text](https://github.com/aaronmkwong/Python-WMA-Retail-Sales-Forecast/blob/main/Images/03_Deasonalized_Sales.JPG)

Of the 3,048 forecasts generated by the program the most and least accurate scenarios (i.e. minimum and maximum MAPE), for each province and category are displayed in a data frame with a colour gradient to highlight their relative performance along with their respective standard deviations. Also, the average and median MAPE across all scenarios are included. 

Alberta Clothes with a 4 month moving average and weights of 0.2, 0.1, 0.1 and 0.6 had both the most accurate forecast with the smallest variation from the average MAPE across the 36 months from 2017 to 2019.          

Alberta Hobby with a 2 month moving average and weights of 0.9 and 0.1 was the least accurate forecast, while Manitoba Hobby with a 2 month moving average and weights of 0.9 and 0.1 had the highest variation from the average.  

![alt text](https://github.com/aaronmkwong/Python-WMA-Retail-Sales-Forecast/blob/main/Images/04_Summary_Statistics_Forecast.JPG)

comments to be entered here

![alt text](https://github.com/aaronmkwong/Python-WMA-Retail-Sales-Forecast/blob/main/Images/05_Error_Distribution.JPG)

comments to be entered here

![alt text](https://github.com/aaronmkwong/Python-WMA-Retail-Sales-Forecast/blob/main/Images/06_Actual_Forecast_MAPE.JPG)

**Data Sources**

Statistics Canada via the Web Data Service (API database access) using the vector IDs specific for clothes and hobby retail sales for the provinces of BC, AB, SK and MB. 
https://www.statcan.gc.ca/eng/developers/wds
