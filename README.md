# Modeling Extreme Weather Risk (2000–2023) 🌪️🌧️🔥

A machine learning + data analysis project that explores global climate and socioeconomic indicators and builds a model to predict **above-baseline extreme weather activity** at the country-year level.

---

## 🔎 Research Goal
**Can we use climate + socioeconomic features to predict whether a country-year will experience “high” extreme weather activity?**

This notebook:
- cleans + explores a multi-country dataset (2000–2023),
- engineers labels for “high extreme events,”
- trains and evaluates classification models,
- interprets drivers with feature importance.

---

## 📌 Key Results (from the notebook)
- Built a baseline **Random Forest classifier** to predict high extreme-weather activity.
- Evaluated performance using **confusion matrix** + **ROC curve**.
- Initial approach produced **AUC ≈ 0.48** (near-random baseline).
- Improved label definition using a **country-relative threshold** (median-based “HighExtreme”) and a better split strategy, increasing performance to **AUC = 0.516**.

> Note: Results depend on label design, split strategy, and feature availability. This project focuses on building a clear, reproducible pipeline and illustrating how target definitions change model performance.

---

## 📊 What’s in the Notebook
### Data work
- Standardizes country + year fields
- Handles missing values and numeric conversions
- Creates derived columns (e.g., extreme events labels)

### EDA / Visualization
- Trend + distribution visualizations (climate + socioeconomic variables)
- Correlation-style comparisons between factors and events

### Modeling
- Baseline classification (Random Forest)
- Evaluation:
  - train/test split
  - confusion matrix
  - ROC curve + AUC
- Interpretation:
  - feature importance ranking

---

## 🧰 Tech Stack
- Python
- Jupyter Notebook
- pandas, numpy
- scikit-learn
- matplotlib (and/or seaborn depending on your notebook)

---

## 📦 Data
This project assumes a country-year dataset with climate and socioeconomic variables (e.g., temperature, CO₂, rainfall, sea level rise, renewables, forest area, population) and an outcome related to extreme weather.

### Expected inputs
If your repo includes a CSV, list it here (examples):
- `climate_extreme_weather_2000_2023.csv`

If the dataset is not included (common for coursework), include:
- where to download it, or
- instructions on how to reproduce it, or
- a note explaining that the dataset was provided for class.

---

## ▶️ How to Run
### 1) Clone the repo
```bash
git clone <YOUR_REPO_URL>
cd <YOUR_REPO_NAME>
