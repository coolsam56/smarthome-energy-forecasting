# SmartHome AI Energy Forecasting

Streamlit dashboard that uses a trained LSTM model to forecast household
electricity consumption from historical readings.

## Run locally

Python 3.11 is recommended.

```bash
python3.11 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
streamlit run app.py
```

The included processed dataset and trained model are loaded from `data/` and
`models/`; no training step is needed to run the dashboard.

## Deploy to Render

Create a Render Blueprint from this repository. Render uses `render.yaml` to
install dependencies and start the Streamlit server. The dataset and model
files must remain committed to the repository because the app loads them at
startup.
