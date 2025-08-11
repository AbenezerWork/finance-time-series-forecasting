# Financial Time Series Forecasting

This project focuses on analyzing and forecasting financial time series data. It provides a framework for fetching historical stock data, performing exploratory data analysis, and preparing the data for time series modeling.

## Features

*   **Data Retrieval**: Fetches historical stock price data using the `yfinance` library.
*   **Exploratory Data Analysis (EDA)**: Includes various EDA techniques to understand the characteristics of the financial data, such as:
    *   Visualizing closing prices over time.
    *   Calculating and plotting daily returns to analyze volatility.
    *   Computing rolling statistics (mean and standard deviation) to identify trends.
*   **Stationarity Testing**: Uses the Augmented Dickey-Fuller (ADF) test to check for stationarity in the time series data.
*   **Risk Analysis**: Calculates Value at Risk (VaR) and the Sharpe Ratio to assess the risk and return of the assets.

## Getting Started

### Prerequisites

*   Python 3.x
*   pip

### Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/AbenezerWork/finance-time-series-forecasting.git
    cd finance-time-series-forecasting
    ```

2.  **Create and activate a virtual environment (recommended):**
    ```bash
    python -m venv .venv
    source .venv/bin/activate
    ```

3.  **Install the required dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

## Usage

The primary analysis is conducted in the Jupyter Notebook located in the `notebooks` directory.

1.  **Start Jupyter Notebook:**
    ```bash
    jupyter notebook
    ```

2.  **Open the notebook:**
    Navigate to `notebooks/data-exploration.ipynb` in the Jupyter interface and open it.

3.  **Run the cells:**
    You can run the cells in the notebook sequentially to see the data analysis and visualizations.

## Project Structure

```
.
├── data/               # Directory for storing raw and processed data
├── models/             # Directory for trained models
├── notebooks/          # Jupyter notebooks for exploration and analysis
│   └── data-exploration.ipynb
├── reports/            # Directory for generated reports or figures
├── src/                # Source code for the project
├── .gitignore          # Files to be ignored by Git
└── requirements.txt    # Project dependencies
```

## Dependencies

The project's dependencies are listed in the `requirements.txt` file:

*   `yfinance`
*   `pandas`
*   `matplotlib`
*   `seaborn`
*   `statsmodels`
