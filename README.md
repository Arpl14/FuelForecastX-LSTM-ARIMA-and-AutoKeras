# ⛽ Petrol Price Forecasting Dashboard


A predictive dashboard that compares LSTM, ARIMA, and AutoML (AutoKeras) models to forecast weekly U.S. petrol prices across three fuel types (`A1`, `R1`, `D1`) using deep learning and time series techniques.
![Untitled design (1)](https://github.com/user-attachments/assets/291ad883-9706-457f-a00a-a4fe26f180df)

---

## 🧩 Project Overview

This project explores multivariate petrol price forecasting using historical fuel price data. It demonstrates how to handle real-world time series, apply model-driven forecasting, and visualize results through an interactive dashboard built with Plotly Dash.

---

## 🔑 Key Features & Challenges

-  **Multivariate Forecasting** for A1, R1, D1 grades  
-  **LSTM**, **ARIMA**, and **AutoKeras** model comparison  
-  **Evaluation Metrics**: RMSE, MAE, R² Score  
-  **Residual Analysis** for error visualization  
-  Handles real-world noise, missing values, and outliers  
-  Interactive **Plotly Dash App** for model insights  

---

## ⚙️ Technical Implementation

- **Languages & Frameworks**: Python, TensorFlow/Keras, scikit-learn, statsmodels, AutoKeras, Plotly, Dash  
- **Key Libraries**: NumPy, Pandas, Matplotlib, Seaborn, Joblib  
- **Techniques Used**:
  - Min-Max Scaling
  - IQR-based Outlier Detection
  - Bidirectional LSTM Networks
  - Rolling Forecasting with ARIMA
  - AutoML Regression using AutoKeras
  - Forecast vs Actual Comparison
  - Model Evaluation & Residual Tracking
- **ATS Keywords**: Time Series Forecasting, LSTM, ARIMA, AutoML, Deep Learning, TensorFlow, Dashboarding, Data Visualization, Python, Plotly Dash, Model Evaluation

---

## ▶️ Project Workflow

1. Load and clean fuel price dataset  
2. Handle missing values and outliers  
3. Scale and split data for training/testing  
4. Build & train models:
   - Bidirectional LSTM (Keras)
   - ARIMA with rolling forecast
   - AutoKeras regression model
5. Save predictions & model artifacts  
6. Compare results in an interactive dashboard  

---

## 🏆 Achievements

- Deployed a full forecasting pipeline from EDA to visualization  
- Integrated traditional, deep learning, and AutoML methods  
- Created a clean, responsive dashboard with Plotly Dash  
- Conducted multi-model evaluation with error visualization  
- Enabled easy extensibility and model comparison

---

## 🚀 How to Use

!pip install jupyter_dash
from jupyter_dash import JupyterDash
app = JupyterDash(__name__)
# [Define your layout here] ( You can use given models, data and scalar )
app.run_server(mode='inline')  # or mode='external'
