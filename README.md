# Project title: Forecasting Walmart Sales with Machine Learning (Kaggle Competition https://www.kaggle.com/competitions/m5-forecasting-accuracy)

The presentation file can be found here: https://github.com/YHL996/walmart-sales-prediction/blob/main/ML_project.pdf

Our goal was to predict the future daily sales of products in Walmart's physical stores and submit our results to Kaggle to evaluate prediction accuracy. We aimed to predict the daily sales for the next 28 days for each product across 10 stores in California, Texas, and Wisconsin. Each store sells around 3,000 products, giving us daily sales data for approximately 30,000 products over more than 5 years. Additionally, we have weekly price data for each product and information on holidays and significant events like the Super Bowl and Christmas.

We approached this as a supervised learning problem, using historical sales, prices, store and product categories, and important events to predict 28-day sales ahead. Our loss function was a mean square error (MSE).

After data preprocessing and feature engineering, our features fall into four categories:

1. Historical sales: lagged sales, moving averages, and standard deviations.
2. Daily product prices: maximum, minimum, and standard deviation over time.
3. Store and product category information.
4. Important events and government assistance program dates.

We tried a variety of models: Gradient Boosting, Neural Networks(CNN, LSTM, Transformer), and Ensemble model.

Our final model was an LSTM model, which had a better evaluation score(weighted root mean squared scaled error (RMSSE)) of 0.686.
