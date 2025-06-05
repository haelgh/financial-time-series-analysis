# Stationarity & Decomposition of Financial Time Series

This project explores the properties of financial time series data through statistical stationarity tests and signal decomposition techniques.  
Implemented in Python using a real-world dataset (VIX – Volatility Index), the work demonstrates key preprocessing and diagnostic tools used in time series forecasting.
The project and its accompanying reports were completed in Ukrainian.
---

## 🧠 Objective

- Assess the stationarity of financial time series using Augmented Dickey-Fuller (ADF) and KPSS tests.
- Decompose time series into trend, seasonal, and residual components using STL.
- Visualize characteristics and identify preprocessing steps before forecasting.

---

## 📊 Dataset

- **Source**: [Kaggle – VIX Index Dataset](https://www.kaggle.com/datasets/alexanderbader/volatility-index-vix)
- **Format**: Daily historical data (open, high, low, close, volume, etc.)

---

## 🛠️ Tools & Libraries

- `pandas` for data manipulation
- `statsmodels` for stationarity tests and STL decomposition
- `matplotlib`, `seaborn` for visualization

---

## 🔬 Methods

- **ADF (Augmented Dickey-Fuller)** — test for unit root (non-stationarity)
- **KPSS (Kwiatkowski-Phillips-Schmidt-Shin)** — complementary test for stationarity
- **STL Decomposition** — seasonal-trend decomposition using LOESS
- **Rolling Mean & Variance** — visual inspection of stationarity

Each result is interpreted and visualized to support preprocessing choices.

---

## 📁 Structure

- `Time_series.ipynb` – full analysis, step by step
- `ЛР2.pdf` – written summary of stationarity analysis 
- `ЛР3.pdf` – report with decomposition insights

---

## 📈 Sample Output

<p align="center">
  <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/30/VIX_1yr.png/800px-VIX_1yr.png" width="600"/>
</p>

> Example image placeholder — replace with your actual plots once uploaded.

---

## 📌 Notes

The project focuses purely on exploratory data analysis and signal understanding. No predictive modeling is included yet.  
It serves as a preparation step for future time series forecasting (e.g., ARIMA, LSTM).

---

## 👤 Author

Created by [Olha Tytarenko](https://www.linkedin.com/in/olha--tytarenko/) as part of coursework in signal processing and time series analysis.

---

## ⚠️ Disclaimer

For academic and demonstrational use only. Dataset sourced from third-party public repository (Kaggle).
