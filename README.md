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

Below are example plots produced during the time series analysis:

- Original VIX time series
<p align="center">
  <img src="https://github.com/user-attachments/assets/dc5e31d0-429b-4c53-b6b1-2a843cc15d9f" alt="VIX Time Series" width="600"/>
</p>

- STL decomposition: trend, seasonality, residuals
  The plot below illustrates the STL decomposition of the VIX index into trend, seasonal, and residual components:

    - **Trend**: captures the long-term movement of the volatility index  
    - **Season**: shows recurring short-term cycles  
    - **Residual**: reflects irregular, unexplained noise 
<p align="center">
  <img src="https://github.com/user-attachments/assets/d017de6f-1947-4d7c-978c-464a47f031ca" alt="STL Decomposition" width="600"/>
</p>

- Rolling mean and variance visualization
  The chart below shows the original VIX time series along with its 30-day rolling mean and standard deviation, used for visual stationarity diagnostics.
<p align="center">
  <img src="https://github.com/user-attachments/assets/505a4a07-d69e-4499-b92a-f59aafcbfd5d" alt="STL Decomposition" width="600"/>
</p>

- ADF and KPSS test statistics
<p align="center">
  <img src="https://github.com/user-attachments/assets/d017de6f-1947-4d7c-978c-464a47f031ca" alt="STL Decomposition" width="600"/>
</p>

> *Note: The project and its accompanying reports were completed in Ukrainian.*

## 📉 Forecasting with ARIMA and GARCH

To evaluate the predictability of VIX dynamics, we implemented both a baseline ARIMA(1,1,1) model and an enhanced ARIMA-GARCH approach.  

Key metrics:
- **MAE** (mean absolute error): 5.54  
- **RMSE** (root mean squared error): 8.64

The GARCH-enhanced model provided improved stability and better captured volatility behavior.

### Forecast Comparison

<p align="center">
  <img src="https://github.com/user-attachments/assets/65efa751-2806-45ae-a814-366f2ba49db2" alt="ARIMA Baseline Forecast" width="700"/>
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/f593bca4-eade-42f3-9349-071591c620fc" alt="ARIMA-GARCH Forecast" width="700"/>
</p>

### Residual Diagnostics

<p align="center">
  <img src="https://github.com/user-attachments/assets/113fde29-d9e2-4d08-9b32-07de315a23e3" alt="ARIMA Residuals" width="600"/>
</p>

These plots indicate that the enhanced ARIMA-GARCH model reduces residual error and better adapts to volatility clustering.

> *Note: Forecasting analysis was performed in Ukrainian and included in the final report.*

---

## 👤 Author

Created by [Olha Tytarenko](https://www.linkedin.com/in/olha--tytarenko/) as part of coursework in signal processing and time series analysis.

---

## ⚠️ Disclaimer

For academic and demonstrational use only. Dataset sourced from third-party public repository (Kaggle).
