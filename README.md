# Airline-Pricing-Intelligence
International Airline Pricing Intelligence
# ✈️ International Airline Pricing Intelligence
### Maximizing US Airline Revenue from International Travelers
Phase 1

---

## 📌 Project Overview

| Field | Details |
|---|---|
| **Project Title** | International Airline Pricing Intelligence |
| **Project Type** | A + F (Forecasting + Decision Product) |
| **Stakeholder** | Revenue management teams at US carriers (Delta, United, American Airlines) |
| **Core Question** | What factors drive international airfare demand and pricing, and how can US airlines optimize pricing strategies to maximize revenue from international routes? |
| **Hypothesis** | Exchange rates, political sentiment, seasonality, and route competition significantly predict international ticket demand — and modeling these can surface pricing opportunities airlines are currently missing |
| **Target Variable** | International ticket price and/or demand (bookings/seat load factor) on international routes |
| **Success Metrics** | MAE and RMSE on price prediction, R², and a demonstrated revenue uplift scenario |

---

## 📂 Repository Structure

```
airline-pricing-intelligence/
│
├── data/                        # Do NOT commit raw data files here
│   └── README.md                # Instructions on how to download the data
│
├── notebooks/
│   ├── 01_data_cleaning.ipynb   # Week 2: Data cleaning + audit
│   ├── 02_eda.ipynb             # Week 2: Exploratory Data Analysis
│   ├── 03_baseline_model.ipynb  # Week 3: Baseline model
│   └── 04_phase1_report.ipynb   # Week 4: Full Phase 1 report
│
├── src/                         # Reusable functions and scripts
│   └── utils.py                 # Helper functions
│
├── outputs/                     # Saved plots, model outputs
│
├── .gitignore                   # Ignores data files, secrets, cache
├── requirements.txt             # All Python dependencies
└── README.md                    # This file
```

---

## 📊 Data Sources

| Dataset | Source | Purpose |
|---|---|---|
| BTS DB1B Survey | [Bureau of Transportation Statistics](https://www.transtats.bts.gov/) | Primary — actual fares paid on international routes |
| FRED Exchange Rates | [Federal Reserve (FRED)](https://fred.stlouisfed.org/) | USD/CAD, USD/EUR, USD/GBP exchange rate features |
| GDELT Project | [GDELT](https://www.gdeltproject.org/) | News sentiment on US travel/immigration policy |
| BTS International Air Traffic | [BTS](https://www.transtats.bts.gov/) | Monthly inbound international traveler volume |

> ⚠️ Raw data files are **not committed** to this repository due to size. See `data/README.md` for download instructions.

---

## ⚙️ Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/YOUR_USERNAME/airline-pricing-intelligence.git
cd airline-pricing-intelligence
```

### 2. Create a Virtual Environment (recommended)
```bash
python -m venv venv
source venv/bin/activate        # Mac/Linux
venv\Scripts\activate           # Windows
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### 4. Download the Data
Follow the instructions in `data/README.md` to download and place datasets in the correct folders.

### 5. Run the Notebooks
Open Jupyter and run notebooks in order (01 → 02 → 03 → 04):
```bash
jupyter notebook
```

---

## 📦 Requirements

All dependencies are listed in `requirements.txt`. Key libraries include:

- `pandas` — data manipulation
- `numpy` — numerical computing
- `matplotlib` / `seaborn` — visualization
- `prophet` — baseline time series forecasting
- `xgboost` — advanced modeling
- `scikit-learn` — model evaluation
- `vaderSentiment` — news sentiment scoring
- `fredapi` — exchange rate data from FRED

---

## 📅 Project Timeline

### Phase 1 (Weeks 1–4)
| Week | Goals |
|---|---|
| Week 1 | Topic finalized, data sources identified, GitHub repo set up |
| Week 2 | Data cleaning, data audit, EDA |
| Week 3 | Feature engineering, baseline model, error analysis |
| Week 4 | Phase 1 report, Phase 2 plan |

### Phase 2 (Weeks 1–12)
| Weeks | Goals |
|---|---|
| 1–2 | Improved features + stronger baseline |
| 3–5 | Model iteration (Prophet → XGBoost → LightGBM) |
| 6–7 | Evaluation, robustness, error analysis |
| 8–9 | Interpretation, fairness, SHAP values |
| 10–11 | Streamlit app / dashboard productization |
| 12 | Final write-up + presentation |

---

## 🤖 AI Usage Log

| Date | Tool | Request Summary | What Was Used | What Was Changed / Verified |
|---|---|---|---|---|

---

## ⚠️ Responsible AI & Ethics Notes

- No personal traveler data is used — all datasets are aggregated public records
- Exchange rate and sentiment data will be clearly documented for reproducibility
- Model limitations and potential biases will be documented in Phase 2

---

## 👤 Author

- **Name:** TODO — Add your name
- **Program:** Data Science Masters
- **Course:** Data Science with AI
- **GitHub:** https://github.com/YOUR_USERNAME

---

*Last updated: March 2026*
