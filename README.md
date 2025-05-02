# 📈 Stock Price Prediction Using Facebook Prophet

Forecasting financial time series is a critical task in the fields of quantitative finance and data science. In this project, we use **Facebook Prophet**, a robust forecasting model developed by Meta, to predict the **stock trading volume** of **Apple Inc. (AAPL)** using historical data from **NASDAQ** between 2018 and 2019.

---

## 📌 Project Objective

The main goal of this project is to:
- Analyze historical stock data of Apple Inc.
- Understand temporal patterns such as trend and seasonality
- Build a forecasting model using Facebook Prophet
- Predict future stock volume
- Visualize the predictions and model components

---

## 🗃️ Dataset

- **Source:** Historical stock data for Apple Inc. (AAPL) from NASDAQ.
- **Period Covered:** 2018 to 2019
- **Features Used:**
  - `Date`
  - `Open`
  - `High`
  - `Low`
  - `Close`
  - `Adj Close`
  - `Volume`

---

## 🔧 Tools & Libraries

- Python 3.x
- Pandas
- NumPy
- Matplotlib / Seaborn
- Statsmodels
- **Facebook Prophet**
  
---

## 📚 Project Workflow

### 1. Exploratory Data Analysis
- Overview of data structure and key statistics
- Visualization of volume and price trends over time
- Boxplots to analyze distribution by months and years
- Durbin-Watson test for autocorrelation

### 2. Data Preprocessing
- Handling datetime formats
- Sorting data chronologically
- Filtering business days using `USFederalHolidayCalendar`
- Creating new date-based features like `Month` and `Year`

### 3. Time Series Decomposition
- Seasonal decomposition of volume using `seasonal_decompose` from statsmodels

### 4. Forecasting with Facebook Prophet
- Prepare the data in Prophet’s expected format (`ds`, `y`)
- Train Prophet on historical stock volume
- Make future predictions and visualize them
- Plot Prophet components: Trend, Weekly and Yearly seasonality

---

## 📊 Key Results

- Facebook Prophet successfully modeled and forecasted stock volume data
- Identified clear **weekly seasonality** and **long-term trends**
- Easy visualization of prediction intervals and component breakdown

---

## 📌 Why Prophet over ARIMA?

This project opted for **Prophet** instead of ARIMA because:
- Prophet automatically detects seasonality and handles missing dates
- It is more intuitive for business-oriented time series like stock market data
- It easily accommodates holidays and irregular intervals

---


## 🚀 Future Work

- Add comparison with **ARIMA/SARIMA** models
- Include other external features (e.g., news sentiment, macroeconomic indicators)
- Evaluate using performance metrics (RMSE, MAE)
- Extend forecasting to `Open` and `Close` prices

---

## 🧑‍💻 Author

**Ashwini Bawankar**  
*Data Science Intern | Passionate about Machine Learning & Forecasting*

---

## 📬 Contact

📧 Email: [abawankar13@gmail.com]  
🔗 LinkedIn: [https://www.linkedin.com/in/ashwini-bawankar/]  


