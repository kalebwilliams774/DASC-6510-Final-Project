# Analysis of Bitcoin (BTC-USD) performance against performance other blue chip stocks: Wal-Mart (WMT), Google (GOOG), General Motors (GM) using typical timeseries models.

Description: Analysis of Bitcoin (BTC-USD) performance against performance other blue chip stocks: Wal-Mart (WMT), Google (GOOG), General Motors (GM) using typical timeseries models.
Authors: Kaleb Williams, Caleb Vonmaydell
 
Final project for DASC 6510 (Time Series Analysis and Forecasting) at Thompson River Univeristy (Fall 2023 semester)

NOTE: Code is written in the format of an rmd (R markdown file) therefore when copying code not using rmd file format exclude exclude the sections containing back tick (`) and anything containing curly braces and the letter "r" ({r}). Each segment contained within those backticks is supposed to run without running all code blocks for those unfamiliar with rmd files.

In order to run the code the required packages must be installed:

install.packages('quantmod') Used to download data from yahoo finance

install.packages('tidyverse') Used for ggplot and various other plotting tools

install.packages('fpp3') Used for timeseries models and other timeseries functions

install.packages('fable.prophet') Used for facebook prophet model

GOAL: To evaluate performance of Bitcoin against other major stocks peformance during pivotal points in recent human history.

Methodology:

This project consists of R code used to analyze the trends in the closing prices of Wal-Mart (WMT), Google (GOOG), General Motors (GM) versus the performance of Bitcoin (BTC-USD) and their volatilities using the fpp3 package tidyverse time series analysis packages.

Volatility definition used was: v = \abs{\sqrt{v}-\sqrt{\hat{v}}}, where is the closing price for the stocks and Bitcoin

Trends were analyzed using the plots of the data over various significant time periods during the course of the last ten years. The COVID-19 pandemic being a focal point of the analysis. Once significant points in time were identified for study time series forecasting models were applied.

Time series forecasting models ARIMA(), ETS() and facebooks prophet model were used to forecast the closing price and volatility of the closing prices of the stocks and Bitcoin.

Once forecasted, accuracies are then calculated to view best forecast for each stock and their volatility. Plots and accuracies being the deciding factor in which forecasting model provided the best results in predicting the actual outcome of the stocks which is then cross-refrenced against Bitcoin's performance.
