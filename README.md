# Quantitative Analysis of Price & Daily Returns

## Overview  
This Jupyter Notebook performs a quantitative analysis of stock price data and daily returns for Amazon (AMZN) from January 2020 to December 2024. The analysis explores:  
- Statistical patterns in daily price fluctuations  
- Momentum or mean-reversion in the asset's movements  
- Modeling the security's path as statistically independent increments  

## Key Questions Explored  
1. Do daily price fluctuations follow predictable statistical patterns?  
2. Is there measurable momentum or mean-reversion in the asset's movements?  
3. Can we model the security's path as statistically independent increments?  

## Setup  

### Libraries Used  
- `yfinance`: Download stock price data  
- `numpy` and `pandas`: Numerical and data manipulation  
- `matplotlib` and `seaborn`: Data visualization  
- `scipy.stats`: Statistical analysis  

### Data Collection  
- **Ticker Symbol**: AMZN (Amazon)  
- **Date Range**: January 1, 2020 to December 31, 2024  
- **Data Columns**: Open, High, Low, Close, Volume  

## Steps  
1. **Environment Setup**: Installed `yfinance` and imported necessary libraries  
2. **Data Download**: Fetched AMZN stock price data and stored in a DataFrame  
3. **Data Exploration**: Verified data structure by displaying the first few rows  
4. **Returns Calculation**: Computed instantaneous rate of return (log returns)  
5. **Visualization**: Plotted daily returns over the last 252 trading days (~1 year)  
6. **Descriptive Statistics**: Generated summary statistics for daily returns  
7. **Statistical Analysis**: Compared return distribution to normal distribution  

## Key Findings  

### Descriptive Statistics  
- Mean daily return: ~0.067%  
- Standard deviation: ~2.266%  
- Minimum return: -15.140%  
- Maximum return: 12.690%  

### Visualization  
- Daily returns plot shows volatility clustering (periods of high/low variability)  

### Statistical Comparison  
- Returns show slight deviations from normal distribution in skewness/kurtosis  

## Conclusion  
This analysis reveals statistical behavior of AMZN's daily returns, providing foundations for exploring:  
- Momentum/mean-reversion effects  
- Price movement independence  
- Advanced modeling (ARIMA/GARCH)  

## How to Use This Notebook  
1. Install required libraries (`!pip install yfinance` if needed)  
2. Run cells sequentially to reproduce analysis  
3. Modify ticker/date range for other analyses  

## Future Work  
- Extend analysis to other stocks/indices  
- Implement advanced statistical tests/models  
- Explore external factor correlations (market indices, news sentiment)  

**Note**: Warnings during `yfinance` installation can be ignored. Analysis focuses on closing prices and log returns for simplicity.  
