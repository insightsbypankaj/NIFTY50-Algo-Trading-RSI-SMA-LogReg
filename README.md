**NIFTY50 Algo-Trading Model (RSI, SMA, Logistic Regression)**
This project builds an automated trading strategy for selected NIFTY50 stocks using
RSI, SMA crossover, and Logistic Regression to generate buy/sell predictions and evaluate trading performance.


**Project Overview**


The goal of this project is to apply data analytics and machine learning techniques to develop a rules-based trading strategy.
Key components include:


        Fetching historical stock data using yfinance
        Feature engineering (RSI, SMA, returns, volatility)
        ML-based prediction using Logistic Regression
        Backtesting trading performance
        Automating buy/sell signals using Google Sheets

        
**Dataset**


       Source: Yahoo Finance (yfinance)
       Stocks used:
       NIFTY 50, INFY, TCS, RELIANCE
       Date range: January 2024 – Present
       Frequency: Daily OHLCV data

**Tech Stack**


      Python
      Pandas, NumPy
      Matplotlib, Seaborn 
      Scikit-learn
      yfinance
      Google Sheets API     

      
**Features Used**


     Simple Moving Averages (SMA)
          SMA 20
          SMA 50
          Used to detect trend direction and crossover signals.

     
**Relative Strength Index (RSI)**


     Used to detect overbought/oversold zones.

     
**Logistic Regression Model**


     Predicts whether the next day price will go up or down.

     
**Strategy Logic**


  Buy signal generated when:

  
     SMA20 crosses above SMA50
     RSI < 30
     Logistic Regression predicts “Up”

     
  Sell signal generated when:
     SMA20 crosses below SMA50
     RSI > 70
     Logistic Regression predicts “Down”

     
**Results**


The model outputs:
     Win rate
     Accuracy
     Precision, Recall, F1-score
     Profit/Loss
     Equity curve
     Confusion matrix

     
**Future Improvements**


     Add LSTM / Random Forest model
     Include more NIFTY50 stocks
     Deploy using Streamlit web app
     Real-time API integration
