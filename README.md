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
- Visualization of volume over time
  ![Screenshot 2025-05-03 002909](https://github.com/user-attachments/assets/53b29f46-18e5-4646-bf1f-cfd74d1e6ca5)
- Boxplots to analyze distribution by months and years
  ![Screenshot 2025-05-03 003946](https://github.com/user-attachments/assets/15baaa8a-8292-4cf5-94d2-912020816b85)
  ![Screenshot 2025-05-03 004007](https://github.com/user-attachments/assets/d5988679-b664-40e5-9836-26e1d97b49f1)
  ![Screenshot 2025-05-03 004028](https://github.com/user-attachments/assets/53672631-d954-4cf0-a9a3-60f507c8f2a4)
- Durbin-Watson test for autocorrelation

### 2. Data Preprocessing
- Handling datetime formats
- Sorting data chronologically
- Filtering business days using `USFederalHolidayCalendar`
- Creating new date-based features like `Month` and `Year`

### 3. Time Series Decomposition
- Seasonal decomposition of volume using `seasonal_decompose` from statsmodels
  ![Screenshot 2025-05-03 001439](https://github.com/user-attachments/assets/2d0fd38d-709d-4d91-a36d-c01b8e5a6220)


### 4. Forecasting with Facebook Prophet
- Prepare the data in Prophet’s expected format (`ds`, `y`)
- Train Prophet on historical stock volume
- Make future predictions and visualize them
- Plot Prophet components: Trend, Weekly and Yearly seasonality
 ![Screenshot 2025-05-03 002106](https://github.com/user-attachments/assets/e98439a2-50ad-49f3-8fc5-82c677fa2c82)
 ![Screenshot 2025-05-03 002128](https://github.com/user-attachments/assets/a05469df-42c4-49cc-8c1f-2d8b4f8e7654)



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


