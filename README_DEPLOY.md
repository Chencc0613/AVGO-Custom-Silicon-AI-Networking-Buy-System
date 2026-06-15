# AVGO Custom Silicon + AI Networking Buy System

Streamlit mobile-style dashboard for AVGO.

## Files

```text
streamlit_app.py
avgo_custom_silicon_buy_system.py
requirements.txt
.streamlit/config.toml
README_DEPLOY.md
```

## Local run

```bash
pip install -r requirements.txt
streamlit run streamlit_app.py
```

## Streamlit Community Cloud

- Main file path: `streamlit_app.py`
- Recommended Python: 3.11 or 3.12
- This app does **not** use `pandas_datareader` or FRED, to avoid Streamlit Cloud compatibility issues.

## Core logic

AVGO is modeled as:

```text
Custom ASIC / XPU demand
+ AI networking
+ hyperscaler AI CapEx
+ VMware / software FCF
+ margin and FCF quality
- customer concentration / geo risk
- valuation and macro risk
```

Manual inputs are intentional because the most important AVGO stock drivers often come from earnings-call commentary, design-win disclosures, ASIC backlog, networking demand, and VMware integration updates that yfinance cannot reliably parse.

Manual execution only. This app never places orders.
