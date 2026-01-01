# 🚲 Bike Sharing Demand Forecasting  
*Using Time Series and Machine Learning Models*

---

## 📘 Project Overview

This project focuses on **forecasting daily bike-sharing demand** using a combination of **time series techniques**, **machine learning**, and **deep learning models**.  
Accurate demand forecasting is essential for **operational efficiency**, **resource allocation**, and **user satisfaction** in urban bike-sharing systems.

The study performs a **comparative analysis** of multiple models to identify the most reliable approach for short-term demand prediction.

---

## 🎯 Objectives

- Analyze historical bike-sharing demand as a time series  
- Identify **trend**, **seasonality**, and **cyclical patterns**  
- Apply statistical, machine learning, and deep learning models  
- Compare models using standard evaluation metrics  
- Determine the most accurate and practical forecasting approach  

---

## 🗂️ Dataset Description

- **Dataset**: Daily Bike Sharing Dataset  
- **Time Period**: 2011 – 2012  
- **Records**: 731 daily observations  
- **Features**:
  - Date
  - Weather conditions
  - Working day / holiday indicators
  - Environmental variables
  - Total bike demand (`cnt`)

---

## 🔍 Exploratory Data Analysis (EDA)

Key analyses performed:

- Time series visualization of daily demand  
- Trend and seasonal behavior analysis  
- Monthly and weekly seasonality inspection  
- STL decomposition (Trend, Seasonality, Residuals)  
- ACF and PACF plots for temporal dependency analysis  
- Rolling mean and rolling standard deviation analysis  

---

## ⚙️ Data Preprocessing

- Converted date column to datetime format  
- Renamed target variable (`cnt → y`)  
- Created dummy variables for categorical features  
- Removed irrelevant attributes  
- Handled missing and inconsistent records  
- Ensured daily time frequency consistency  

---

## 🤖 Models Implemented

The following models were developed and evaluated:

### 📌 Statistical Models
- **SARIMAX** – Captures autoregression and seasonal effects  
- **Holt-Winters** – Exponential smoothing with trend and seasonality  

### 📌 Machine Learning Models
- **Random Forest Regressor** – Captures nonlinear relationships and feature interactions  

### 📌 Deep Learning Model
- **LSTM (Long Short-Term Memory)** – Learns long-term temporal dependencies  

### 📌 Time Series Framework
- **Prophet** – Decomposes trend, seasonality, and holiday effects with interpretability  

---

## 📏 Evaluation Metrics

Models were evaluated using:

- **RMSE (Root Mean Square Error)**  
- **MAPE (Mean Absolute Percentage Error)**  

These metrics assess both absolute and relative forecasting accuracy.

---

## 📊 Results Summary

| Model           | RMSE   | MAPE (%) | Observation |
|-----------------|--------|----------|-------------|
| SARIMAX         | 1716.84 | 35.98 | Weak seasonality capture |
| Holt-Winters    | 1436.07 | 28.89 | Good seasonal tracking |
| Prophet         | 3880.10 | 15.94 | Smooth but high RMSE |
| LSTM            | 1051.82 | 20.67 | Strong temporal learning |
| **Random Forest** | **953.38** | **18.04** | **Best overall performance** |

---

## 🔮 Forecasting Insights

- Strong **upward trend** observed across the dataset  
- Clear **weekly and yearly seasonality**  
- Higher demand during **summer months and weekends**  
- Random Forest and LSTM closely follow actual demand patterns  
- Prophet provides high interpretability but smoother forecasts  

---

## 🧪 Technologies and Tools

- **Python**
- **Pandas**, **NumPy**
- **Matplotlib**, **Seaborn**
- **Statsmodels**
- **Scikit-learn**
- **TensorFlow / Keras**
- **Prophet**
- **Google Colab**

---
## 📘 Key Learnings

- Practical understanding of time series forecasting  
- Comparative evaluation of classical and modern forecasting models  
- Importance of seasonality and external influencing factors  
- Trade-off between model interpretability and predictive accuracy  

---

## 🏁 Conclusion

The study concludes that the **Random Forest** model provides the best predictive accuracy for bike-sharing demand forecasting, while **LSTM** effectively captures long-term sequential dependencies.  
A hybrid approach combining **statistical model interpretability** with **machine learning robustness** can further enhance real-world deployment and decision-making reliability.

---

## 📜 License

This project is intended for **academic and educational purposes**.  
Reuse is permitted with appropriate attribution.

---


## 📁 Project Structure

