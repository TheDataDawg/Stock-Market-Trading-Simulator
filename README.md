# Stock Market Trading Simulator

This project is a stock market trading simulator that uses real-time prices from AlphaVantage and simulates trading strategies via the Alpaca API.

It implements three strategies:
- **Mean Reversion**
- **Simple Moving Average**
- **Bollinger Bands**

Each strategy runs on historical daily adjusted closing prices and can optionally place simulated orders using the Alpaca paper trading API.

## Features
- Fetches historical stock data from AlphaVantage
- Calculates and applies trading strategies
- Optionally submits simulated trades using Alpaca
- Appends trade results to a results file

## Requirements
- Python 3.7+
- See `requirements.txt` for Python dependencies

## Setup

### Clone this repository
```
git clone https://github.com/yourusername/stock-trading-simulator.git
cd stock-trading-simulator
```

### Install dependencies
```
pip install -r requirements.txt
```

### Create a `config.json` file in the project root
```
{
  "APCA_API_KEY_ID": "YOUR_ALPACA_KEY",
  "APCA_API_SECRET_KEY": "YOUR_ALPACA_SECRET",
  "ALPHAVANTAGE_API_KEY": "YOUR_ALPHA_KEY"
}
```
*Do not commit `config.json` to version control.*

## Run the simulator
```
python main.py
```
(*or whatever your main file is named*)

## Notes
- Results are saved to `/home/ubuntu/environment/final_project/results.json`
- Data files are saved in `/home/ubuntu/environment/final_project/data/`
- Make sure you have valid API keys for both AlphaVantage and Alpaca.
