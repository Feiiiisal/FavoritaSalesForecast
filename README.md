# FavoritaSalesForecast

## Introduction:
Predicting grocery sales might sound simple, but with a vast inventory and multiple variables at play, it becomes a unique puzzle. For Corporación Favorita, a leading grocery chain, accurately forecasting sales is crucial. Whether it's avoiding disappointed customers due to stock-outs or reducing waste from unsold items, having a precise forecast makes a difference.

This project dives deep into the sales data, seeks patterns, and crafts a prediction system to give the most accurate sales forecast possible.

## Getting Started:
### Prerequisites:
To run the analysis and scripts provided, ensure you have the following packages installed:

'pandas'
'pyodbc'
'python-dotenv'
'matplotlib'
'seaborn'
'plotly'
'nbformat'
'statsmodels'
'dash'
'wordcloud'
'keras'
'Cython'
'tensorflow'
'keras-tuner'
'pmdarima'
'scikeras'
You can easily install these packages using pip:


### Data Sources:
Our dataset resides in three main places:

SQL Database
OneDrive
GitHub
To load the datasets from these sources, we used pyodbc for SQL database connections and pandas for reading CSV files.

## Project Structure:
The main sections of our analysis include:

Data Acquisition: Connecting to multiple databases, transforming raw data into usable Pandas DataFrames.
Exploratory Data Analysis (EDA): Visualization and statistical analysis of oil prices, holiday events, and transaction datasets.
Time Series Analysis: Employing ARIMA and SARIMAX models to forecast sales over time.
Neural Network Modeling: Using LSTM networks to learn from historical sales data.
Model Evaluation: Assessing the performance of models with metrics like RMSE.

## Results:
The analyses provided insights like:

Trends in oil prices over time.
Understanding the role of holidays and events on sales.
Patterns in transaction volume across stores and over time.
Predicting future sales with the help of various models.

## How to Run the Code:
After cloning the repository, navigate to the project directory and run the main script:

## Acknowledgments:
Special thanks to the team members who contributed to this project and Corporación Favorita for providing the dataset.

Note: Remember to always keep your environment variables and any sensitive information secure and never push them to public repositories.

Happy Forecasting!

