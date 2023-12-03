# Analysis of Bitcoin (BTC-USD) performance against performance other blue chip stocks: Wal-Mart (WMT), Google (GOOG), General Motors (GM) using exponential smoothing during the COVID-19 pandemic.

Authors: Kaleb Williams, Caleb Vonmaydell

NOTE: Code is written in the format of an rmd (R markdown file) therefore when copying code not using rmd file format exclude exclude the sections containing back tick (`) and anything containing curly braces and the letter "r" ({r}). Each segment contained within those backticks is supposed to run without running all code blocks for those unfamiliar with rmd files.

Final project for DASC 6510 (Time Series Analysis and Forecasting) at Thompson River Univeristy (Fall 2023 semester)

Description: Analysis of Bitcoin (BTC-USD) performance against performance other blue chip stocks: Wal-Mart (WMT), Google (GOOG), General Motors (GM) using typical timeseries models. For the sake of this project we will be using exponential smoothing methods from the fpp3 package and testing accuracy in forecasting the volatility of the daily closing price of the blue chip stocks Wal-Mart (WMT), Google (GOOG) and General Motors (GM) against Bitcoin (BTC-USD).

 In order to run the code the required packages must be installed:

install.packages('quantmod') Used to download data from yahoo finance

install.packages('tidyverse') Used for ggplot and various other plotting tools

install.packages('fpp3') Used for timeseries models and other timeseries functions

GOAL: To evaluate performance of Bitcoin against other major stocks peformance during the COVID-19 pandemic.

Methodology:

This project consists of R code used to analyze the trends in the closing prices of Wal-Mart (WMT), Google (GOOG), General Motors (GM) versus the performance of Bitcoin (BTC-USD) and their volatilities using the fpp3 package, tidyverse time series analysis packages and quantmod package.

Volatility definition used was: v = \abs{\sqrt{v}-\sqrt{\hat{v}}}, where is the closing price for the stocks and Bitcoin.

Trends were analyzed using the plots of the data over the COVID-19 pandemic and stock data from 2004 to 2023.

Time series forecasting model ETS() was used to forecast the closing price volatility of the stocks and Bitcoin.
