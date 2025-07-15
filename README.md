# 📈 Stock Price Prediction using LSTM

Predict future stock prices using historical data and Long Short-Term Memory (LSTM) neural networks. This project demonstrates a full workflow from data collection to model evaluation, using the POWERGRID.NS stock as an example.

## 📝 Overview

This notebook guides you through:
- Downloading and preparing stock data
- Visualizing trends and patterns
- Building and training an LSTM model for time series forecasting
- Evaluating and visualizing predictions

## 📊 Dataset

- **Source:** Yahoo Finance via `yfinance`
- **Stock:** POWERGRID.NS
- **Period:** January 1, 2000 – November 1, 2024
- **Attributes:** Open, High, Low, Close, Volume

## 🧰 Tools & Libraries

- Python 3.7+
- Jupyter Notebook
- pandas, numpy
- matplotlib, plotly
- yfinance
- scikit-learn
- tensorflow, keras

## ⚙️ Installation

Install all dependencies with:
```bash
pip install pandas numpy matplotlib plotly yfinance scikit-learn tensorflow
```

## 📌 Workflow

1. **Data Collection**  
   - Download historical stock prices using `yfinance`.

2. **Data Preprocessing**  
   - Handle missing values
   - Normalize data with `MinMaxScaler`
   - Create sequences for LSTM input

3. **Data Visualization**  
   - Plot Open, Close, High, Volume
   - Interactive candlestick charts with Plotly

4. **Model Building**  
   - Train an LSTM model on closing prices
   - Use 100 timesteps for sequence prediction

5. **Prediction & Evaluation**  
   - Test model on 30% of data
   - Inverse-transform and plot predictions

## 📈 Results

- The LSTM model captures trends in closing prices.
- Visual comparison between actual and predicted prices is provided.
- (Optional: Add metrics such as RMSE or MAE if available.)

## 🚀 Usage

1. Open `stock.ipynb` in Jupyter Notebook or JupyterLab.
2. Run all cells in order.
3. To use a different stock, change the ticker symbol in the notebook.
4. Adjust model parameters (timesteps, epochs, etc.) as needed.

## 💡 Notes

- The notebook is set up for POWERGRID.NS but can be adapted for other stocks.
- Results may vary depending on market volatility and chosen parameters.