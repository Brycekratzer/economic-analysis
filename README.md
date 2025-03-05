# Economic Analysis and Market Forecasting Toolkit

## Overview

This notebook provides a comprehensive framework for analyzing economic indicators, market trends, and their relationships across different time periods. It's designed for financial analysts, economists, and data scientists who want to explore connections between economic fundamentals and market performance, with special focus on normalizing data across different reporting frequencies and creating composite economic health metrics.

## Features

### Data Collection and Preparation
- Imports financial market data (S&P 500, Dow Jones, NASDAQ) using yfinance
- Collects economic indicators from FRED database (GDP, CPI, interest rates, employment metrics)
- Adjusts historical data for inflation to enable true apples-to-apples comparisons
- Handles different data reporting frequencies (daily, weekly, monthly, quarterly)

### Analysis Techniques
- **Time-based Normalization**: Both short-term (rolling window) and long-term methods using RobustScaler for outlier resistance
- **Market Classification**: Categorizes market movements into 43 distinct classes for granular trend analysis
- **Composite Indicators**: Creates economic health scores using weighted combinations of key metrics
- **Feature Engineering**: Develops specialized metrics like Housing Stress, Financial Stress, and Crash Risk

### Visualization Tools
- Time series plotting with flexible date range selection
- Comparative timeline analysis to contrast similar historical periods
- Multi-metric visualization for correlation analysis

## Key Components

1. **Inflation Adjustment**: Converts all monetary values to current dollars using CPI data
2. **Normalization Methods**: 
   - Short-term: Uses rolling windows appropriate to each data frequency
   - Long-term: Normalizes against all available historical data
   - Divergence analysis: Compares short vs. long term perspectives

3. **Economic Health Metrics**: Weighted combinations of:
   - Employment indicators (30%)
   - Production & business activity (20%)
   - Consumer behavior (15%)
   - Housing market (15%)
   - Financial markets (20%)

4. **Risk Assessment Models**: 
   - Market pressure analysis at 30, 90, and 150-day intervals
   - Economic stress evaluation across multiple timeframes
   - Composite crash risk indicator with time-weighted components

## Usage Examples

The notebook demonstrates several practical applications:

1. Comparing 2021-2025 market conditions with the 2006-2008 financial crisis
2. Tracking housing market stress over extended periods
3. Evaluating economic health using multiple normalization techniques
4. Developing early warning indicators for market instability

## Requirements

- Python libraries: pandas, numpy, matplotlib, yfinance, pandas_datareader, pandas_ta, scikit-learn
- Access to FRED API and Yahoo Finance data
- Basic understanding of economic indicators and financial markets

## Getting Started

Begin by running the data collection cells to import market data and economic indicators. The notebook structure follows a logical progression from data gathering through normalization to analysis and visualization, with each section building on previous components.

For customized analysis, focus on the feature engineering section where you can develop specialized metrics tailored to specific research questions or investment strategies.
