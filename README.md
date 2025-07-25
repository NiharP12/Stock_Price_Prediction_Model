# Stock_Price_Prediction_Model

# Project Objective:

To build a robust and interpretable stock price prediction system for Reliance Industries Ltd. using a combination of:

- Power BI for real-world data cleaning, transformation, and preprocessing.

- Python & Machine Learning to engineer features, train regression models, and evaluate performance.

The objective is to predict the next day's closing price using historical stock data and visualize key market patterns that influence stock behavior. This project demonstrates an end-to-end data science workflow from data wrangling to model deployment.

#  PowerBI Role:

In this project, Power BI was used for:

- Cleaning raw stock market data

- Transforming and standardizing column data types

- Handling missing values using built-in Power Query features

- Removing irrelevant or duplicate rows (if any)

- Exporting the cleaned dataset as reliance_cleaned.csv for ML processing

# Python & Machine Learning Role:

In the Python phase of this project:

- Converted original features into previous-day lag features (e.g., Prev_Close, Prev_Open, etc.)

- Dropped unnecessary columns that don't contribute to prediction

- Created two new features:

  - Prev_Range: difference between High and Low

  - Prev_Return_%: % change from previous close

- Trained and evaluated two regression models:

  - Linear Regression (Scikit-learn)

  - XGBoost Regressor

- Compared both models based on:

  - Accuracy

  - R² Score

  - RMSE (Root Mean Squared Error)

- Found that Linear Regression outperformed XGBoost
  - ✔️ Linear Regression

    - Accuracy: 99.24%

    - R² Score: 0.99

    - RMSE: 6.14

  - ❌ XGBoost Regressor

    - Accuracy: 98.87%

    - R² Score: 0.99

    - RMSE: 7.47

- Plotted Actual vs Predicted close prices using Linear Regression

  ![LinePlot](https://github.com/user-attachments/assets/17039ca9-4799-49df-8808-bf2dda291424)


# Conclusion:

In this project, we successfully built an end-to-end stock price prediction system for Reliance Industries by combining the data cleaning power of Power BI with the predictive capabilities of Machine Learning in Python.

Key outcomes:

- Power BI was used to clean raw stock data, transform data types, and export a structured dataset.

- Python was used to engineer features, train regression models, and evaluate performance.

- We implemented and compared two models:

  - Linear Regression (Accuracy: 99.24%, RMSE: 6.14)

  - XGBoost Regressor (Accuracy: 98.87%, RMSE: 7.47)

- Despite XGBoost’s complexity, Linear Regression performed better on this dataset, showing that simple models can be highly effective with well-prepared data.

- The final prediction results were visualized using scatter plots and trend lines, demonstrating strong alignment between actual and predicted prices.

This project proves that with clean data and proper feature engineering, traditional ML models can provide accurate and reliable predictions — even in volatile domains like stock markets.
