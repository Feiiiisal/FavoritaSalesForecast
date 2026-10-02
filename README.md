# Favorita Store Sales Forecasting

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
![Python](https://img.shields.io/badge/python-3.9%2B-blue)
![Models](https://img.shields.io/badge/models-ARIMA%20%7C%20LSTM%20%7C%20XGBoost-green)
![Power BI](https://img.shields.io/badge/dashboard-Power%20BI-yellow)

Forecasting daily grocery sales for **Corporación Favorita**, a large retailer
in Ecuador. Accurate forecasts help a retailer avoid empty shelves and reduce
waste from unsold stock. This project explores the sales data, tests several
forecasting approaches and compares them. The best model is deployed in the
companion app
[SalesForecastStreamlitApp](https://github.com/Feiiiisal/SalesForecastStreamlitApp).

## What's in the project

- **Data acquisition**: the data comes from a SQL database, OneDrive and this
  repository, loaded with `pyodbc` and `pandas`.
- **Exploratory analysis**: oil prices over time, the effect of holidays and
  events on sales, and transaction patterns across stores and time.
- **Time series models**: ARIMA and SARIMAX (`statsmodels`, `pmdarima`).
- **Machine learning and deep learning**: XGBoost and LSTM networks
  (`tensorflow`/`keras`, tuned with `keras-tuner`).
- **Evaluation**: RMSE and RMSLE, including cross-validated splits.
- **Dashboard**: a Power BI report in `Power BI Dashboard/sales_dashboard.pbix`.

## Results

With tuned parameters, the XGBoost model reached an **RMSLE of about 0.0054**
in the notebook's evaluation. The full comparison of models is in
`store_sales_forecasting.ipynb`.

## Repository contents

```
store_sales_forecasting.ipynb   The analysis and modelling notebook
Datasets/                       holidays_events, oil, stores, transactions, train.zip, test
Power BI Dashboard/             Power BI report (.pbix)
requirements.txt
```

`Datasets/train.zip` must be unzipped before the training data can be read.
`store_sales_forecasting (1).ipynb` is a second copy of the notebook.

## Setup

```bash
pip install -r requirements.txt
jupyter notebook store_sales_forecasting.ipynb
```

Some of the data is read from an Azure SQL database using credentials from a
`.env` file. Never commit `.env`; if you do not have database access, use the
CSV files in `Datasets/`.

## Acknowledgements

Thanks to the team members who worked on this project, and to Corporación
Favorita for providing the data.

## License

[MIT](LICENSE)
