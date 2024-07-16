# Predicting stock performance with Long Short-Term Memory (LSTM)

## Overview

This project leverages Long Short-Term Memory (LSTM) networks to predict performance of various stocks, sector indices and market indices. The analysis uses stock prices for IBM, Apple, American Express, JPMorgan Chase, Exxon Mobil and Occidental Petroleum. Sector Indices include Financial Sector Index, Technology Sector Index and Energy Sector Index. Market indices include GDP, SP500 and Unemployment Data. 

The project covers Data Collection and Preprocessing, Explanatory Data Analysis (EDA), Univariate-, Bivariate-, and Multivariate Time Series Analysis, Time Series Decomposition, Stationary and Autocorrelation Tests, Feature Engineering, and the training of LSTM models to forecast variable prices.

## Table of Contents

1. Project Description
2. Data Sources
3. Variables
4. Features
5. Setup
6. Usage
7. Results
8. Contributing
9. License

## Project Description

This repository contains an R project that predicts stock performance using LSTM models. The project is documented in a Jupyter Notebook, covering steps from data collection and preprocessing to exploratory data analysis (EDA) and LSTM model training.

Goal of the project was to analyze stock market performance using time series analysis and build predictive models using LSTM modeling to forecast stock prices.

## Data Sources

### Stocks
IBM, Apple, American Express, JPMorgan Chase, Exxon Mobil, and Occidental Petroleum Data from Yahoo Finance.

### Sector Indices
Financial Sector Index, Technology Sector Index, and Energy Sector Index Data  from Yahoo Finance.

### Market Indices
GDP and Unemployment Data from the Federal Reserve Economic Data (FRED) database. SP500 from Yahoo Finance.

## Variables

Multiple variables in code are presented as their ticker symbol.

**$IBM** IBM                                     

**$AAPL** Apple                                    

**$AXP** American Express                         

**$JPM** JPMorgan Chase                           

**$XOM** Exxon Mobil                              

**$OXY** Occidental Petroleum   


**$XLF** Financial Sector Index

**$XLK** Technology Sector Index

**$XLE** Energy Sector Index


**$GSPC** SP500

**$GDP** GDP

**$UNRATE** Unemployment Rate


All stocks, sectors and SP500 have six columns; Open, High, Low, Close, Volume and Adjusted.

**Open**: The price at which the stock first traded upon the opening of the exchange on a given day.

**High**: The highest price at which the stock traded during the day.

**Low**: The lowest price at which the stock traded during the day.

**Close**: The price at which the stock last traded upon the close of the exchange on a given day.

**Volume**: The total number of shares traded during the day.

**Adjusted**: The closing price adjusted for dividends, stock splits, and other corporate actions to provide a more accurate reflection of the stock's value over time.


## Features

**Data Collection and Preprocessing**: Scripts for gathering and cleaning stock, sector, and market index data, ensuring it is ready for analysis.

**Exploratory Data Analysis (EDA)**: Initial analysis to understand data characteristics, distributions, and potential patterns.

**Univariate Time Series Analysis**: Analysis of individual time series (e.g., stock prices) to identify trends, seasonality, and other characteristics.

**Bivariate Time Series Analysis**: Examination of relationships between two time series (e.g., comparing stock prices of IBM and Apple).

**Multivariate Time Series Analysis**: Analysis involving multiple time series to uncover complex interactions among variables (e.g., stocks, sectors, and market indices).

**Time Series Decomposition**: Breaking down time series data into its component parts (trend, seasonality, residuals) for better understanding and modeling.

**Stationary and Autocorrelation Tests**: Statistical tests to determine if the time series is stationary and to measure the correlation of the series with its past values.

**Feature Engineering**: Creation of new features from raw data, such as lagged values, moving averages, and other statistical features to enhance model performance.

**LSTM Model Training**: Development, training, and tuning of Long Short-Term Memory (LSTM) networks to forecast stock and index prices based on the processed data.


## Setup

Follow these steps to set up on run the project:

1. Clone the Repository
- Clone the GitHub repository to your local machine:

  git clone https://github.com/yourusername/your-repository.git
  cd your-repository

2. Install Jupyter Notebook
- If you don’t have Jupyter Notebook installed, you can install it using pip:

  pip install notebook

3. Install R

- Download and install R from the CRAN website

4. Install Required R Packages and IRkernel

- Open R and install the necessary packages including the IRkernel, which allows       Jupyter to run R code:

  install.packages(c("IRkernel", "keras3", "tidyverse", "cluster", "dtw",             "dtwclust")) IRkernel::installspec(user = FALSE)






















