# Cryptocurrency Price Prediction for the Next 30 Days

This project uses machine learning with time series models to forecast Bitcoin closing prices for the next 30 days. The notebook uses Yahoo Finance for data collection, supports candlestick plotting, and leverages AutoTS and Prophet for advanced forecasting.

## Features

- **Data Collection:** Downloads BTC-USD price history with yfinance.
- **Preprocessing & Visualization:** Cleans and flattens data columns, handles missing values, and plots interactive candlestick charts with Plotly.
- **Modeling:** Uses AutoTS and Prophet to forecast future prices. All column names and arguments are updated for pandas compatibility.
- **Analysis:** Computes correlations and trends using up-to-date column names.
- **Export & Plot:** Saves results and visualizes both historical and predicted prices.

## Usage Instructions

1. Install dependencies:
pip install -r requirements.txt

2. Run the notebook in Jupyter, VS Code, or Google Colab.
3. The notebook will download BTC data, visualize it, and forecast future closing prices.
4. You can easily fit new models by adjusting code and parameters as needed.

## Important Notes

- All code and visualization sections use updated pandas/Plotly syntax.
- For concatenating Series, use `pd.concat`, **not** `.append`.
- When using AutoTS, supply correct column names: e.g., `'Date_'` and `'Close_BTC-USD'`.
- For visualization, always use actual DataFrame column names after any renaming or flattening.
- If running on Python 3.11+, use `prophet` (not `fbprophet`).

## Author & License

- Notebook and code by a final-year BTech student.
- MIT License.
