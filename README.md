# Finance Time Series Forecasting and Portfolio Optimization

This project explores time series forecasting of financial assets and uses the forecasts to construct and backtest optimal portfolios. It uses a combination of statistical models (SARIMAX) and deep learning models (LSTM) for forecasting, and `PyPortfolioOpt` for portfolio optimization.

## Getting Started

### Prerequisites

- Python 3.13
- pip

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/AbenezerWork/finance-time-series-forecasting.git
   ```
2. Navigate to the project directory:
   ```bash
   cd finance-time-series-forecasting
   ```
3. Create a virtual environment:
   ```bash
   python -m venv .venv
   ```
4. Activate the virtual environment:
   ```bash
   source .venv/bin/activate
   ```
5. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

### Usage

The project is organized into Jupyter notebooks in the `notebooks/` directory.

- **`notebooks/data-exploration.ipynb`**: This notebook covers data loading, cleaning, and exploratory data analysis. It also includes stationarity tests and the calculation of risk metrics like Value at Risk (VaR) and the Sharpe Ratio.
- **`notebooks/model-development.ipynb`**: This notebook is for training and evaluating forecasting models. It includes feature engineering with technical indicators, training a SARIMAX model, and a multi-variate LSTM model.
- **`notebooks/forcasting-and-optimization.ipynb`**: This notebook focuses on generating forecasts and using them to construct optimal portfolios. It uses `PyPortfolioOpt` to find the optimal portfolio for both maximum Sharpe ratio and minimum volatility, and visualizes the efficient frontier.

## Project Structure

```
├── data/
│   └── processed/
├── models/
├── notebooks/
│   ├── data-exploration.ipynb
│   ├── model-development.ipynb
│   └── forcasting-and-optimization.ipynb
├── reports/
├── src/
├── .gitignore
├── README.md
└── requirements.txt
```

- **`data/`**: Contains the raw and processed data.
- **`models/`**: Stores the trained models and scalers.
- **`notebooks/`**: Contains the Jupyter notebooks for data analysis, modeling, and optimization.
- **`reports/`**: For saving reports and visualizations.
- **`src/`**: For source code (if any).

## Dependencies

- yfinance
- pandas
- matplotlib
- seaborn
- statsmodels
- numpy
- cython
- scikit-learn
- scipy
- statsforecast
- tensorflow
- pandas_ta
- joblib
- PyPortfolioOpt