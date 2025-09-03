

# Forecasting & Stochastic Models

Interactive notebooks for teaching and learning classical forecasting (ARIMA/ETS), regression-based time-series, and stochastic modeling. Each chapter is a self-contained notebook with data, exercises, and takeaway checkpoints.

[![Open in Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/waelrash1/forecastingmodelsPY/HEAD)

---

## Quickstart

### Option A — Conda (recommended)
```bash
# 1) create env (uses environment.yml pinned for teaching)
conda env create -f environment.yml
conda activate forecastingmodels

# 2) launch Jupyter
jupyter lab   # or: jupyter notebook

python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate
pip install -r requirements.txt
jupyter lab

jupyter nbconvert --to notebook --execute CH01/CH01.ipynb


CH01/ … CH11/      # chapter notebooks (teaching units)
CH04.ipynb         # top-level convenience copies (to be moved into chapter dirs)
CH05.ipynb
files/             # shared assets (images, etc.)
environment.yml    # reproducible conda env for teaching
requirements.txt   # pip alternative (generated from env)
LICENSE            # Apache-2.0
