# SVM_SVR
 using SVR and technical indicators for stock price prediction


This Jupyter notebook utilizes a machine learning approach to predict stock prices. It focuses on using Support Vector Regression (SVR) models
optimized through a grid search strategy to forecast future values of stock prices based on historical data.

Key libraries used in this notebook include 
`pandas` for data manipulation,
`matplotlib` and `seaborn` for data visualization,
`numpy` for numerical operations, `scipy` for statistical tests,
`sklearn` for modeling and evaluation of the regression models.

The notebook includes a variety of functions to automate the analysis:
- **`prepare_data()`**: Prepares and cleans the dataset for modeling.
- **`calculate_technical_indicators2()`**: Computes various technical indicators used as features for the models.
- **`train_model()`**: Trains the SVR model using grid search to find the best parameters.
- **`make_predictions()`**: Generates predictions using the trained model.
- **`visualize_held_stocks()`**: Visualizes the performance of the stocks over a period.

### Detailed Explanation

The notebook begins by importing stock data from an Excel file, cleaning the data, and then calculating technical indicators like Moving Average Convergence Divergence (MACD),
Exponential Moving Averages (EMA), Bollinger Bands, Relative Strength Index (RSI), and Stochastic Oscillator. These indicators serve as input features for the machine
learning model.

A significant part of the notebook involves defining and using the `train_model()` function, which applies a `GridSearchCV` with a `TimeSeriesSplit` to optimize the
SVR parameters. This approach is particularly suited for time series data like stock prices, ensuring that the model is not only accurate but also robust against overfitting.

Predictive performance is assessed using metrics such as Mean Absolute Percentage Error (MAPE) and Mean Squared Error (MSE), ensuring the model's effectiveness in practical
scenarios.

Visualization functions are utilized extensively to display the results of the analysis, including the performance of the held stocks and the technical indicators over time.
This visual feedback is crucial for interpreting the model's behavior and for making informed decisions based on the predictions.

Warnings are suppressed throughout the notebook to ensure clarity and readability of the output, focusing on the essential results. Additionally, performance metrics
such as returns, volatility, and others are calculated to provide a comprehensive view of the investment's potential outcome based on historical data.

Overall, the notebook is a robust tool for predicting stock prices, equipped with detailed statistical analysis and machine learning model optimization, aimed at
providing actionable insights into stock market investments.