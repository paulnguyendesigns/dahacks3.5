# Currency Exchange API 💱

A simple Flask API for currency conversion and historical exchange rate data, powered by ExchangeRate-API and FreeCurrencyAPI.

## Features
- `GET /convert?base=USD&target=EUR&amount=100` — Convert an amount between currencies
- `GET /api/currencies` — List available currencies
- Historical exchange rate lookups

## Tech Stack
- **Language:** Python
- **Framework:** [Flask](https://flask.palletsprojects.com/)
- **Other Libraries:** [Flask-CORS](https://flask-cors.readthedocs.io/), [python-dotenv](https://pypi.org/project/python-dotenv/)
- **External APIs:** [ExchangeRate-API](https://www.exchangerate-api.com/), [FreeCurrencyAPI](https://freecurrencyapi.com/)

## Setup
1. Install dependencies:
   ```bash
   pip install flask flask-cors python-dotenv
   ```
2. Create a `.env` file with:
   ```
   EXCHANGE_API_KEY=your_exchangerate_api_key
   HISTORICAL_API_KEY=your_freecurrencyapi_key
   ```
3. Run the app:
   ```bash
   python app.py
   ```
4. Visit `http://localhost:5000` to see available endpoints.
