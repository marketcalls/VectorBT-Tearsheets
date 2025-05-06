# VectorBT Tearsheets

**VectorBT Tearsheets** is a Python project that combines backtesting with [VectorBT](https://github.com/polakowo/vectorbt) and tear sheet reporting using [QuantStats](https://github.com/ranaroussi/quantstats). It features a full backtest of an EMA crossover strategy on RELIANCE.NS and compares its performance against NIFTY 50.

## Project Structure

```
VectorBT-Tearsheets/
│
├── docs/                # Documentation or notes
├── tearsheets/          # QuantStats HTML output reports
├── venv/                # Virtual environment (ignored)
├── requirements.txt     # Python dependencies
├── .gitignore           # Git ignore rules
└── README.md            # Project overview
```

## Features

- Download stock data using `yfinance`
- Implement an EMA crossover strategy using `vectorbt`
- Simulate trades with capital, fees, and signal logic
- Generate professional-grade performance reports with `QuantStats`
- Compare strategy returns against NIFTY 50 index

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/marketcalls/VectorBT-Tearsheets.git
cd VectorBT-Tearsheets
```

### 2. (Optional) Create a virtual environment

```bash
python -m venv venv
# On Windows
venv\Scripts\activate
# On macOS/Linux
source venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the strategy script

```bash
python strategy.py
```

### 5. View the results

Open the HTML tear sheet generated in the `tearsheets/` folder using any browser.

## Requirements

- Python 3.8+
- pandas
- numpy
- yfinance
- quantstats
- vectorbt
- plotly

## Notes

- Includes compatibility patches for recent pandas and QuantStats versions.
- Strategy uses an EMA(2) / EMA(27) crossover on RELIANCE.NS.

## Author

[marketcalls](https://github.com/marketcalls)
