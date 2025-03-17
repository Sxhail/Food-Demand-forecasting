# 📊 Food Demand Forecasting using Time Series Analysis  

This project focuses on **time series forecasting** for food demand using **ARIMA and SARIMA models**. We analyze historical data, perform feature engineering, and optimize models to predict future demand accurately.  

---

## 🚀 Project Overview  
### **🔹 Goal:**  
- To build a predictive model that forecasts weekly food demand based on historical data.  
- Improve supply chain management and reduce food wastage.  

### **🔹 Techniques Used:**  
- **Time Series Analysis** (Trend, Seasonality, Stationarity)  
- **Statistical Tests** (ADF Test for Stationarity)  
- **Feature Engineering** (Log Transformations, Seasonal Adjustments)  
- **ARIMA & SARIMA Models** for Forecasting  
- **Error Metrics** (MAE, RMSE, MAPE)  
- **Data Visualization** (Matplotlib, Seaborn, Plotly)  

---

## 📂 Dataset Information  
- **Source:** [Kaggle: Food Demand Forecast Dataset](#)  
- **Files in Dataset:**  
  - `train.csv` → Historical demand data  
  - `fulfilment_center_info.csv` → Warehouse details  
  - `meal_info.csv` → Meal type and category  
- **Key Features:**  
  - `id` → Unique identifier  
  - `week` → Weekly time series data  
  - `center_id` → Warehouse location  
  - `meal_id` → Type of food  
  - `num_orders` → Number of orders placed  
- **Target Variable:** `num_orders` (food demand)  

---

## 🔬 Methodology  
### **1️ Data Preprocessing**  
- Handling missing values and outliers  
- Feature extraction (seasonality, promotions)  
- Log transformations for variance stabilization  
- Checking **stationarity** using **Augmented Dickey-Fuller (ADF) Test**  

### **2️ Time Series Analysis**  
- Identifying **trends, seasonality, and cyclic patterns**  
- Visualizing historical demand using **rolling mean and decomposition**  

### **3️ ARIMA Model Implementation**  
- Checking stationarity and applying **differencing**  
- Training the ARIMA model and forecasting future demand  

### **4 Model Evaluation**  
- Comparing ARIMA and SARIMA models  
- Evaluating performance using:  
  - **Mean Absolute Error (MAE)**  
  - **Root Mean Squared Error (RMSE)**  
  - **Mean Absolute Percentage Error (MAPE)**  

---

## 📈 Visualization & Insights  
🔹 **Demand Trends:**  
- Demand increases in specific months due to **seasonality**.  
- Some fulfillment centers have **higher order volume** than others.  

🔹 **Feature Importance:**  
- Promotions significantly affect demand.  
- Week number and location influence order volume.  

🔹 **Forecasting Plot:**  
- Red line: **Predicted demand**  
- Blue line: **Actual demand**  
- Model is stable and captures trends effectively.  

---

## 📊 Model Performance  
| Model  | MAE  | RMSE  | MAPE |
|--------|------|------|------|
| ARIMA  | 2.8  | 3.03 | 2.44% |

📌 **Best Model:** ARIMA (Lower RMSE and MAPE)  

---

