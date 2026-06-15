# AVGO Streamlit App

Build: AVGO_FUNDAMENTAL_OVERRIDE_V2_2026_06_15

## Files

- `streamlit_app.py`
- `avgo_custom_silicon_buy_system.py`
- `requirements.txt`
- `.streamlit/config.toml`

## Local run

```bash
pip install -r requirements.txt
streamlit run streamlit_app.py
```

## Streamlit Cloud

Main file path:

```text
streamlit_app.py
```

This version avoids `pandas_datareader` and FRED dependencies. It uses yfinance market proxies and includes manual valuation / margin overrides for cases where yfinance returns `NA` for AVGO PE, EPS, or margins.
