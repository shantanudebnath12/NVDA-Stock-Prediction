# NVDA Stock Price Prediction using Random Forest

## Project Overview

This project aims to predict whether NVIDIA Corporation (NVDA) stock price will increase or decrease the next day using a Random Forest classifier. The model uses historical stock data to make predictions based on various technical indicators. I personally have been following NVDA hype on r/wallstreetbets way too much, so thought I would make this quick project.

## Purpose

The main purposes of this project are:

1. To demonstrate the application of machine learning in financial markets.
2. To explore the use of the Random Forest algorithm for binary classification in a time series context.
3. To evaluate the effectiveness of using technical indicators for short-term stock price movement prediction.
4. To showcase data preprocessing, model training, and evaluation skills in a real-world scenario.

## Methodology

1. **Data Collection**: Used yfinance to fetch historical NVDA stock data.
2. **Data Preprocessing**: 
   - Calculated daily returns
   - Created technical indicators (5-day and 20-day Moving Averages, RSI, Volume Change)
   - Prepared the target variable (1 if tomorrow's price is higher, 0 otherwise)
3. **Feature Engineering**: Selected relevant features for the model
4. **Model Training**: Used Random Forest Classifier with default hyperparameters
5. **Evaluation**: Assessed model performance using precision, recall, and F1-score

## Results

The model achieved the following performance metrics:

- Precision: 0.5217
- Recall: 0.4842
- F1-score: 0.5022

These results indicate that the model's performance is only slightly better than random guessing. This outcome is not unusual in the context of stock price prediction due to the complex and often unpredictable nature of financial markets.

## Key Takeaways

1. **Challenging Nature of Stock Prediction**: The results underscore the difficulty of predicting short-term stock price movements, even with machine learning techniques.

2. **Importance of Feature Engineering**: While basic technical indicators were used, more sophisticated features might improve model performance.

3. **Model Limitations**: The Random Forest model, while good at capturing non-linear relationships, may not fully capture the temporal dependencies in stock price data.

4. **Market Efficiency**: The results somewhat support the efficient market hypothesis, suggesting that predicting price movements based solely on historical data is challenging.

5. **Learning Experience**: Despite modest predictive performance, the project provided valuable experience in data preprocessing, model implementation, and evaluation in a financial context.

## Future Improvements

1. Experiment with more advanced feature engineering techniques
2. Implement hyperparameter tuning to optimize the Random Forest model
3. Explore time series-specific models like ARIMA or LSTM networks
4. Incorporate fundamental analysis data or sentiment analysis for a more comprehensive approach
5. Implement a backtesting framework to assess model performance over time

## Disclaimer

This project is for educational purposes only. The model's performance is not sufficient for real-world trading decisions. Always consult with financial experts and perform thorough research before making any investment decisions.
