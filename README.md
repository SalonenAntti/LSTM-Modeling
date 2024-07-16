# Predicting stock performance with Long Short-Term Memory (LSTM) using R

## Overview

This project leverages Long Short-Term Memory (LSTM) networks to predict performance of various stocks, sector indices and market indices. The analysis uses stock prices for IBM, Apple, American Express, JPMorgan Chase, Exxon Mobil and Occidental Petroleum. Sector Indices include Financial Sector Index, Technology Sector Index and Energy Sector Index. Market indices include GDP, SP500 and Unemployment Data. 

The project covers Data Collection and Preprocessing, Explanatory Data Analysis (EDA), Univariate-, Bivariate Time Series Analysis, Time Series Decomposition, Stationary and Autocorrelation Tests, Feature Engineering, training of LSTM models to forecast variable prices and evaluation of these models.

The project as a whole is documented in this repository as **"LSTM.ipynb"** where you can find all project areas mentioned above.

## Table of Contents for the project

**Preparation**: Installing all needed packages for the project.

**Data Collection and Preprocessing**: Scripts for gathering and cleaning stock, sector, and market index data, ensuring it is ready for analysis.

**Exploratory Data Analysis (EDA)**: Initial analysis to understand data characteristics and to provide statisical understanding of the variables.

**Univariate Time Series Analysis**: Analysis of individual time series to identify trends, seasonality, and other characteristics throughout the review period. Focus on closing prices.

**Bivariate Time Series Analysis**: Examination of relationships between variables. Methods used: Correlations heatmaps and cross-correlation to identify dependencies and lagged relationships. Focus on closing prices.

**Time Series Decomposition**: Breaking down time series data into its component parts (trend, seasonality, residuals) for better understanding the time series. Focus on closing prices.

**Stationary and Autocorrelation Tests**: Statistical tests to determine if the time series is stationary and to measure the correlation of the series with its past values. With stationary and utocorrelation Tests, determination of modeling algorithm was done. Focus on closing prices.

**Feature Engineering**: Creation of new features from raw data. Feature included lagged values, moving averages and combination of these to include statistical features to enhance model performance.

**LSTM Model Training**: Development, training, and tuning of Long Short-Term Memory (LSTM) networks to forecast stock and index prices based on the processed data. Visualized actual vs predicted values are from best models for each variables. Each variable was tested with variety of different model combinations, such as different type and amount of layers, added features and hyperparameter tuning values.

**Results**: Evaluation of LSTM model performances.

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
<br>
All stocks, sectors and SP500 have six columns; Open, High, Low, Close, Volume and Adjusted.
<br>
<br>
**Open**: The price at which the stock first traded upon the opening of the exchange on a given day. Presented in dollar unit.

**High**: The highest price at which the stock traded during the day. Presented in dollar unit.

**Low**: The lowest price at which the stock traded during the day. Presented in dollar unit.

**Close**: The price at which the stock last traded upon the close of the exchange on a given day. Presented in dollar unit.

**Volume**: The total number of shares traded during the day. Presented in dollar unit.

**Adjusted**: The closing price adjusted for dividends, stock splits, and other corporate actions to provide a more accurate reflection of the stock's value over time. Presented in dollar unit.

**GDP** is presented in billions of dollars, **Unemployment Rate** as a percentage, **SP500** as a point value.


## Setup

Follow these steps to set up on run the project:

**1. Clone the Repository**
- Clone the GitHub repository to your local machine:

  git clone https://github.com/yourusername/your-repository.git
  cd your-repository

**2. Install Jupyter Notebook**
- If you don’t have Jupyter Notebook installed, you can install it using pip:

  pip install notebook

**3. Install R**

- Download and install R from the CRAN website

**4. Install Required R Packages and IRkernel**

- Open R and install the necessary packages including the IRkernel, which allows       Jupyter to run R code:

  install.packages(c("IRkernel", "keras3", "tidyverse", "cluster", "dtw",             "dtwclust")) IRkernel::installspec(user = FALSE)

**5. Run Jupyter Notebook**

- Start Jupyter Notebook from the terminal

  "jupyter notebook"

**6. Open and Run Notebooks**

- In Jupyter Notebook, navigate to the .ipynb file in your project directory and       open it.
- Select the R kernel for the notebook (Kernel > Change kernel > R).

**7. Follow instructions of the Notebook**

- Follow the instructions in the Jupyter Notebook to download and preprocess the       data as needed for the analysis.
- Adjust any model parameters and hyperparameters as specified in the notebook to      fit your analysis requirements.



# Usage

By following instructions of the notebook and running the codes, the notebook performs all tasks mentioned above, including EDA, Training the LSTM model using the provided scripts and Evaluating and analyzing the model's performance for example.

However there are a few changable parts in the code to provide different output for visualization. These are mentioned in that specific code. Feel free to change and try them out.

# Results

The project includes visualizations comparing predicted vs. actual stock prices and performance metrics. Detailed results and discussions are provided in the Jupyter Notebook.

# Contributing

Contributions to this project are welcome. Please fork the repository and submit a pull request with your proposed changes.

# License

This project is licensed under the MIT License.

















