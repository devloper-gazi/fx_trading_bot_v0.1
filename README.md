# FX Trading Bot Template

This repository contains a Python template for an FX (foreign exchange) trading bot that uses Selenium to automate web interactions with a broker’s website. It fetches market data via Yahoo Finance (using the `yfinance` package), computes a simple moving-average crossover strategy, and simulates placing a buy or sell order on the broker's website.

> **IMPORTANT DISCLAIMER:**  
> **This code is provided for educational purposes only.**  
> Automated trading is highly risky, and no simple script (or bot) can guarantee profits or work without continuous maintenance. This template is meant to illustrate one approach to automation when a broker does not provide an API.  
> **Before using this bot with live funds, you must:**
> - Thoroughly test it on a demo account.
> - Modify element selectors, URLs, and logic to match your broker’s website.
> - Ensure you comply with your broker's terms of service.
> - Implement robust error handling and risk management.
> 
> **Use at your own risk.**

## Features

- **Market Data Fetching:** Uses `yfinance` to download live data for the EUR/USD pair.
- **Simple Trading Strategy:** Implements a basic moving-average crossover strategy.
- **Automated Browser Interaction:** Uses Selenium to log in and simulate trade order placement.
- **Modular Design:** The script is organized into functions for login, data retrieval, signal generation, and order placement.

## Requirements

- Python 3.8 or later
- [Selenium](https://pypi.org/project/selenium/)
- [yfinance](https://pypi.org/project/yfinance/)
- [pandas](https://pypi.org/project/pandas/)
- A web browser (Chrome) and corresponding [ChromeDriver](https://chromedriver.chromium.org/)
  
You can install the Python dependencies with:
```bash
pip install selenium yfinance pandas
