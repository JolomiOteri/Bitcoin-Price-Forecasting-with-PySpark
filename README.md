# ₿ Bitcoin Price Forecasting with PySpark

## 📌 Project Overview

This project implements a distributed time-series forecasting pipeline using PySpark to predict future Bitcoin closing prices from historical cryptocurrency market data.

The project demonstrates how distributed machine learning can be applied to financial forecasting by transforming time-series data into a supervised learning problem and training predictive regression models.

The workflow includes data preprocessing, temporal feature engineering, model training, evaluation, and forecasting.

---

## 🎯 Objectives

The objectives of this project are to:

- Forecast Bitcoin closing prices using historical market data
- Create lag-based and rolling statistical features
- Apply distributed machine learning using PySpark
- Compare Linear Regression and Gradient Boosted Trees models
- Evaluate forecasting performance using industry-standard metrics
- Demonstrate FinTech analytics and time-series modelling techniques

---

## 🛠 Technologies Used

- Python
- PySpark
- Spark MLlib
- Pandas
- NumPy
- Databricks
- Google Colab

---

## 📂 Dataset

The project uses historical Bitcoin market data containing:

- Timestamp
- Open Price
- High Price
- Low Price
- Close Price
- Trading Volume

### Target Variable

- Close Price

The objective is to predict future Bitcoin closing prices using historical market behaviour.

---

## 🔄 Project Workflow

### 1. Data Loading

- Load Bitcoin historical market data
- Create a Spark DataFrame
- Inspect schema and data quality

### 2. Data Preprocessing

- Convert timestamps into datetime format
- Organise data chronologically
- Remove missing values
- Aggregate daily observations

### 3. Temporal Feature Engineering

Time-series features were generated using Spark Window Functions.

#### Lag Features

- Lag 1 Day
- Lag 3 Days
- Lag 7 Days
- Lag 14 Days
- Lag 30 Days

#### Rolling Statistics

- 7-Day Moving Average
- 14-Day Moving Average
- 7-Day Rolling Standard Deviation
- 14-Day Rolling Standard Deviation

#### Market Indicators

- Daily Return
- 7-Day Return

---

## 🤖 Models Implemented

### Linear Regression

A baseline forecasting model used to establish benchmark performance.

### Gradient Boosted Trees (GBT)

A more advanced ensemble model capable of capturing nonlinear relationships within financial time-series data.

---

## 📊 Model Evaluation

Models were evaluated using:

- Root Mean Squared Error (RMSE)
- Mean Absolute Error (MAE)
- R² Score

These metrics provide insight into forecasting accuracy and model effectiveness.

---

## 📈 Forecasting Pipeline

```text
Historical Bitcoin Data
          ↓
Data Cleaning
          ↓
Temporal Feature Engineering
          ↓
Lag Features
          ↓
Rolling Statistics
          ↓
Feature Vectorisation
          ↓
Train-Test Split
          ↓
Linear Regression / GBT
          ↓
Forecasting
          ↓
Performance Evaluation
```

---

## 🏦 FinTech Applications

This project demonstrates practical applications in:

- Cryptocurrency Forecasting
- Financial Analytics
- Quantitative Finance
- Risk Analysis
- Trading Strategy Support
- Decision Support Systems

---

## 📈 Skills Demonstrated

- Time-Series Forecasting
- Feature Engineering
- PySpark Machine Learning
- Distributed Computing
- Regression Modelling
- FinTech Analytics
- Cryptocurrency Data Analysis
- Performance Evaluation

---

## ▶️ Running the Project

### Install Dependencies

```bash
pip install pyspark
```

### Run the Notebook

1. Open the notebook in Databricks or Google Colab
2. Install required dependencies
3. Load the Bitcoin dataset
4. Run all notebook cells sequentially
5. Review forecasting results and model performance

---

## 📁 Repository Structure

```text
Bitcoin-Price-Forecasting-PySpark/
│
├── Week10_Group10_AdithyaKumarSridhar.ipynb
├── README.md
└── Dataset/
```

---

## 🚀 Future Improvements

- Hyperparameter tuning
- Cross-validation for time-series forecasting
- XGBoost implementation
- LSTM neural networks
- Prophet forecasting
- Real-time cryptocurrency forecasting dashboards

---

## 👨‍💻 Author

**Jolomi Oteri**

Petroleum Engineer | MSc AI & Data Science Candidate

This project demonstrates distributed financial forecasting using PySpark and machine learning techniques for cryptocurrency price prediction.
