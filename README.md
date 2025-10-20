# 🍷 Wine Sales Forecasting using Time Series Analysis

This project focuses on analyzing and forecasting wine sales data for **ABC Estate Wines** in the 20th century. The goal is to uncover sales trends, evaluate multiple forecasting models, and generate accurate predictions for future sales using time series techniques.

---

## 📘 Overview
As a data analyst at ABC Estate Wines, I aimed to explore historical wine sales data, identify seasonality and trends, and develop robust forecasting models to guide future business planning and decision-making.

---

## 🧩 Key Steps

### 1. Data Preparation & Visualization
- Imported and structured the dataset as a time series.
- Visualized long-term trends and seasonality using **Matplotlib** and **Seaborn**.

### 2. Exploratory Data Analysis (EDA)
- Performed decomposition to separate **trend**, **seasonality**, and **residuals**.
- Derived insights into peak sales periods and sales patterns over time.

### 3. Model Development & Evaluation
- Split data into **training and test sets** (test starting from 1991).
- Built multiple forecasting models:
  - **Exponential Smoothing**
  - **Naïve Forecast**
  - **Regression Models**
  - **ARIMA / SARIMA**
- Evaluated models using **Root Mean Square Error (RMSE)**.

### 4. Stationarity Testing
- Conducted **ADF Test** at α = 0.05 to check stationarity.
- Applied differencing and transformations to achieve stationarity where required.

### 5. Model Optimization & Automation
- Implemented **Automated ARIMA/SARIMA** parameter tuning using **AIC** minimization.
- Compiled a summary table comparing model parameters and RMSE performance.

### 6. Forecasting & Insights
- Forecasted **12 months** of future wine sales with **confidence intervals**.
- Provided recommendations for inventory and production strategy based on forecast trends.

---

## 🧠 Key Learnings
- End-to-end experience in **time series forecasting workflow**.
- Strong understanding of **model selection**, **evaluation**, and **interpretability**.
- Hands-on practice with **ARIMA/SARIMA** models and performance metrics.

---

## ⚙️ Tech Stack
- **Python**
- **Pandas**, **NumPy**
- **Matplotlib**, **Seaborn**
- **Statsmodels**
- **Scikit-learn**

---

## 📊 Results
| Model Type | Parameters | RMSE (Test) | Comments |
|-------------|-------------|--------------|-----------|
| Naïve Forecast | - | 120.45 | Baseline |
| Exponential Smoothing | Trend + Seasonality | 85.12 | Better fit |
| ARIMA (auto) | (1,1,1) | 72.35 | Optimal model |
| SARIMA (auto) | (2,1,1)(1,0,1,12) | **65.48** | Best performer |

---

## 🚀 Future Work
- Integrate automated hyperparameter tuning with `pmdarima`.
- Experiment with **Prophet** and **LSTM-based forecasting models** for comparison.

---
