# Forecasting-USD-TRY-Exchange-Rates-Time-Series-Data-Analysis-and-Preparation

# Time Series Analysis and Predictive Modeling

This project delivers a comprehensive time series analysis and forecasting framework for USD/TRY exchange rates, using advanced statistical techniques.

# Key Highlights

**Statistical Tests & Diagnostics**: Stationarity checks (ADF, KPSS), trend analysis (Hodrick-Prescott filter), and Kruskal-Wallis tests for median differences.
**Exploratory Data Analysis (EDA)**: STL Decomposition for trend and seasonality, and insights on price trends, moving averages, and volatility metrics.
**Predictive Modeling**: ARIMA and SARIMA models with optimized parameters, validated using TimeSeriesSplit and cross-validation.
**Model Comparison**: In-depth evaluation with Ljung-Box tests and confidence interval visualizations for reliable forecasts.
**Backtesting & Performance**: Rolling-window backtesting to assess model stability (ARIMA) and trend sensitivity (SARIMA), highlighting key trade-offs in forecasting.
This project is ideal for anyone looking to apply rigorous time series forecasting methods to real-world financial data, blending data analysis with advanced model evaluation.

# 1. Project Structure
Time Series Data Analysis and Preparation - Covers data retrieval, preprocessing, and exploratory analysis.

# 2. About The Dataset
The dataset consists of daily USD/TRY exchange rate data retrieved from Yahoo Finance. This dataset includes key price metrics like:

Open, High, Low, Close prices
Volume of trades
Adjusted Close for split or dividend-adjusted prices

# 3. Data Preprocessing
**Date Parsing and Feature Engineering**: Extracted features like month, day, year, and seasonal flags to capture temporal trends.
**Technical Indicators**: Included moving averages (SMA_20, SMA_50) to identify short and long-term trends.
**Missing Value Handling**: Addressed missing data by custom imputation methods to avoid distortions, particularly for moving averages.

# 4. Exploratory Data Analysis (EDA)
The analysis notebook dives into a detailed EDA of the dataset to understand the underlying trends, seasonality, and volatility of USD/TRY exchange rates. Key visualizations include:

**Yearly and Monthly Price Analysis**: Visualizes long-term and short-term patterns in exchange rates.
**Moving Averages and Price Differences**: Highlights volatility and trend strength over time.
**High-Low and Close-Open Price Comparisons**: Explores the daily range and fluctuations.
**STL Decomposition**: Breaks down the series into trend, seasonal, and residual components to capture periodic patterns in the data.

# 5. Data Diagnostics and Statistical Tests
Before modeling, several statistical tests were applied to assess stationarity, seasonality, and trend, helping in informed model selection:

**Augmented Dickey-Fuller (ADF) Test**: Assesses the stationarity of the series.
**Kwiatkowski-Phillips-Schmidt-Shin (KPSS) Test**: Provides a complementary stationarity check.
**Kruskal-Wallis Test**: Determines the significance of observed seasonal differences.
**Hodrick-Prescott (HP) Filter**: Separates the cyclical component from the trend for deeper insights into macroeconomic cycles.
