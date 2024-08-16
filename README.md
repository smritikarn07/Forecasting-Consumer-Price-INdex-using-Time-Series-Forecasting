# Forecasting-Consumer-Price-Index-using-Time-Series-Forecasting

## Motivation
I wanted to see whether the **unemployment rate**, **real personal income**, **Fed Funds rate** and **stock price index** have any historical relationship with inflation. 

Economists often refer to the Phillips Curve, showing a trade-off between inflation and **unemployment**. Looking at the data we have plotted below, the trade-off holds true? 
Do stock markets have any predictive power for inflation? **S&P500** is used as Composite index to derive its relationship with inflation.
The Fed Reserve lowers inflation by raising interest rates. Is the **Fed Funds rate** useful for prediction?

In the project, we have tried to answer all these questions.

## Model Framework
* Macroeconomic Variables:
  ![image](https://github.com/user-attachments/assets/e27b8cc8-df65-46ab-b90c-373dd444342d)
  ![image](https://github.com/user-attachments/assets/fb37e9e4-8984-4ddd-beb2-f8b1595d241e)

* Decomposition of Real Personal Income
![image](https://github.com/user-attachments/assets/6236bc53-438e-407f-a770-67c6accf17fa)

* Decomposition of Unemployment Rate
![image](https://github.com/user-attachments/assets/c3123f7e-94c6-4460-aafb-50befa7ccb0c)

* Decomposition of Stock Price Index (S&P 500)
![image](https://github.com/user-attachments/assets/e2bb827c-29bf-4798-9af6-6859906a9130)

* Decomposition of Consumer Price Index (CPI)
![image](https://github.com/user-attachments/assets/a2606789-87d3-4782-989e-0c44e3ecb707)

* Decomposition of Fed Funds Rate
![image](https://github.com/user-attachments/assets/ea9934fa-1662-4b2d-9606-a5cd43a05436)

## Results
### Tests: 
* Stationarity Tests:
![Screenshot (133)](https://github.com/user-attachments/assets/6a2314cd-4004-434f-afb6-85f64c0a95d0)

* Cointegration Tests:
  ![Screenshot (134)](https://github.com/user-attachments/assets/6f733bd7-7462-45ce-abfd-7578fa0f96ce)

### In Sample Forecast Results
![Screenshot (135)](https://github.com/user-attachments/assets/76ad57f2-de6d-4f25-ba33-d3604cad972b)
![Screenshot (136)](https://github.com/user-attachments/assets/b8031f6c-b097-43c3-a352-29eec05f017f)


## OBSERVATION
* Despite some outliers, there appears a curved negative relation between the **unemployment rate** and inflation, providing some visual evidence for the Phillips Curve. This relation is broken down into various subsamples below. 

* There's no clear relationship between **stock markets** and inflation, contrary to popular beliefs.
* There appears to be a positive upward-sloping relationship between the **Fed Funds rate** and inflation. This is not surprising, given that monetary policy responds to inflation (and vice versa).

**Explanation for Outliers:** Outliers may be explained by trends across 1970 and 1980. 
* In the 70s, the US economy experienced high inflation. The clustering of low inflation values from 1980-1999 may correspond to the recession of the 1980s, following aggressive interest rate hikes by the Fed in response to the high inflation in the 70s. **Great Depression.**
* Similarly the **Great Recession** in 2008-2009 had a similar impact on US economy
