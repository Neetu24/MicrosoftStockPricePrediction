# 📈 Microsoft Stock Price Prediction with Machine Learning

## 🧠 Objective

The goal of this project is to develop a time-series forecasting model to predict Microsoft's (MSFT) stock prices using various machine learning and deep learning techniques. We leverage historical stock data and technical indicators to train models like Linear Regression, Random Forest, XGBoost, and LSTM.

---

## 📂 Dataset

- **Source:** Yahoo Finance (`yfinance`)
- **Stock:** Microsoft Corporation (MSFT)
- **Duration:** January 2010 to December 2024

---

## 🛠️ Tools & Libraries Used

- **Python**
- **Pandas, NumPy** – Data manipulation
- **Matplotlib, Seaborn** – Data visualization
- **scikit-learn** – ML preprocessing, models, evaluation
- **XGBoost** – Gradient boosting model
- **TensorFlow / Keras** – Deep learning (LSTM)
- **yfinance** – Data acquisition

---

## 📋 Project Workflow

### 1. Data Collection & Exploration
- Downloaded Microsoft stock data using `yfinance`.
- Explored stock prices and trends.

### 2. Data Preprocessing
- Converted date to `datetime` format and set it as the index.
- Handled missing values using interpolation.
- Normalized features using `MinMaxScaler`.

### 3. Feature Engineering
- Calculated:
  - **SMA** (Simple Moving Average)
  - **EMA** (Exponential Moving Average)
  - **Bollinger Bands**
  - **RSI** (Relative Strength Index)

### 4. Exploratory Data Analysis (EDA)
- Visualized trends, seasonality, and volume correlation.
- Analyzed relationships between indicators and stock price.

### 5. Model Training
- Trained four models:
  - Linear Regression
  - Random Forest Regressor
  - XGBoost Regressor
  - LSTM (Deep Learning)

### 6. Evaluation Metrics
- **MAE (Mean Absolute Error)**
- **RMSE (Root Mean Squared Error)**
- **R² Score (Coefficient of Determination)**

### 7. Forecasting
- Used the trained LSTM model to predict the next **30 days** of stock prices.
- Plotted the forecast alongside historical data.

---

## 📊 Results

- All models were evaluated on unseen test data.
- **LSTM** provided the most accurate results in forecasting future stock trends due to its ability to learn temporal dependencies.

---

## 🔮 Future Enhancements

- Implement Transformer-based models (like GPT or BERT for time series).
- Incorporate additional financial indicators (MACD, OBV, etc.).
- Use sentiment analysis from financial news to boost prediction accuracy.

---

## 📁 File Structure
📦 microsoft-stock-prediction/
┣ 📜 stock_prediction.py ← Main script (or .ipynb)
┣ 📊 stock_forecast_plot.png ← Output plot (optional)
┣ 📄 README.md ← This documentation
