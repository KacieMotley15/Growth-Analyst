
# Mercado Sales Forecast

## Overview

This repository contains code and data files for analyzing and forecasting sales data for Mercado, a fictional company. The analysis utilizes the Facebook Prophet time series forecasting model to predict future sales trends.

## Table of Contents

- [Overview](#overview)
- [Data](#data)
- [Analysis](#analysis)
- [Results](#results)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Overview

The goal of this analysis is to forecast sales for Mercado using historical sales data and identify potential trends or patterns that can inform decision-making.

## Data

The analysis uses two main datasets:
- `mercado_daily_revenue.csv`: Contains daily sales figures for Mercado, quoted in millions of US dollars.
- `mercado_stock_price.csv`: Contains historical stock prices for Mercado.

## Analysis

The analysis consists of the following steps:

### 1. Data Preparation

The sales data and stock price data are loaded into Pandas DataFrames. The necessary transformations are applied, such as setting the date column as the Datetime Index.

### 2. Exploratory Data Analysis

The data is visualized using hvPlot to gain insights into sales trends and stock price movements.

### 3. Time Series Modeling

The Prophet model from the Facebook Prophet library is applied to the sales data. The model is fitted to the data and used to make future sales predictions.

### 4. Forecasting

The Prophet model is used to forecast sales for a specified period, such as the next quarter. The forecasted values for upper and lower bounds are also generated, allowing for the estimation of best-case, worst-case, and most likely scenarios.

## Results

The analysis reveals the following key findings:

- Sales Trends: The analysis of historical sales data shows fluctuations and potential seasonality in Mercado's revenue. Certain periods exhibit higher sales figures, while others show a decline.

- Stock Price Correlation: The correlation analysis between sales data and stock price data suggests a moderate relationship between the two variables. Changes in stock prices may have some influence on sales trends.

- Sales Forecast: The Prophet model provides forecasts for future sales, including best-case, worst-case, and most likely scenarios. These predictions can help inform decision-making and resource allocation for the finance division.

## Usage

To reproduce the analysis, follow these steps:

1. Install the required dependencies listed in the sectio below.
2. Run the Jupyter Notebook `analysis.ipynb` to execute the analysis steps.
3. Review the generated plots and analysis results.





## Packages Used:
import pandas as pd

import holoviews as hv

from fbprophet import Prophet

import hvplot.pandas

import datetime as dt

%matplotlib inline





