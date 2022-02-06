# Stock Analysis
Analysis of stock market data from 2017 and 2018

## Overview

In this analysis, the client initially desired a quick and easy way to identify two indicators of performance ("total volume" and "return") for twelve companies in the US stock market. Total volume is based on the amount of trades for a company's stock in 2017 and 2018. The return percentage reflects the stock's fluctuations (increase or decrease) for a single year.

After establishing this basic code, we refractored the code to loop through all the data at one time to enable the VBA script to run faster. This will enable to script to run faster for larger datasets (aka the entire stock market, not just twelve companies).

## Results

### 2017 compared to 2018

Between 2017 and 2018, all but three companies varied in their return. Only one company (TERP) produced negative yields in 2017 and 2018, while ENPH and RUN were the only two companies with positive returns. The other nine companies had positive gains in 2017 and negative gains in 2018. 

### Run Times

The purpose of refractoring the code was to improve run-time. I confirmed that refractoring decreased the run-time by 82% for 2018 and 72% for 2017. 

Original Run Time for 2017 (0.5546875 s)

Refractored Run Time for 2017 (0.15625 s)

Original Run Time for 2018 (0.5742188 s)

Refractored Run Time for 2018 (0.1054688 s)

## Summary

While refractoring your code can decrease the run time, it is not necessary to obtain the required data. In our analysis, having the code loop through the data once, instead of twelve times (once for each company) produced a more sophisticated code that allowed the data to be accessed more quickly. That said, we needed to have the knowledge of how to efficiently refractor the data (using a ticker index). Refractoring is beneficial to provide a cleaner, easier to use code for clients and colleagues but not necessary to gather the data needed. 
