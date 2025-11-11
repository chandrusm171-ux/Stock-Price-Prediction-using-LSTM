# 📈 Stock Price Prediction using LSTM

This repository contains a Jupyter Notebook that demonstrates how to build, train, and evaluate a **Long Short-Term Memory (LSTM)** neural network for **stock price prediction**.  
The model uses historical stock data downloaded from **Yahoo Finance**, processes it for supervised learning, and visualizes predicted vs. actual prices.

---

## 🧠 Project Overview

This notebook walks through the following major steps:

1. **Data Collection** – Fetches historical stock prices using the `yfinance` API.  
2. **Preprocessing** – Normalizes data and prepares time-series sequences for model input.  
3. **Model Building** – Creates an LSTM network using **TensorFlow/Keras**.  
4. **Training & Evaluation** – Trains the model, monitors performance, and evaluates results using MAE and RMSE.  
5. **Visualization** – Plots predicted and actual stock prices for comparison.

The notebook can be easily adapted for any stock symbol supported by Yahoo Finance.

---

## ⚙️ Requirements

Ensure you have **Python 3.8+** and **Jupyter Notebook** installed.  
Install dependencies using:

```bash
pip install numpy pandas matplotlib yfinance scikit-learn tensorflow
```

---

## 🚀 How to Use

1. **Clone this repository**

   ```bash
   git clone https://github.com/<your-username>/<repo-name>.git
   cd <repo-name>
   ```

2. **Launch Jupyter Notebook**

   ```bash
   jupyter notebook 26c56c99-1637-4f8e-8dc0-d8fb28e2748a.ipynb
   ```

3. **Run all cells** in the notebook.

   The notebook will:
   - Download data for a chosen stock (default: **AAPL**)
   - Train an LSTM model
   - Generate evaluation metrics
   - Plot predictions vs. actual prices

4. **Modify parameters** in the “User Settings” section:
   ```python
   TICKER = "AAPL"
   START_DATE = "2025-01-01"
   SEQ_LENGTH = 60
   EPOCHS = 30
   ```
   Adjust these values to test different stocks or configurations.

---

## 📊 Output

After running the notebook, you will obtain:

- Model training & validation loss curves
  <img width="700" height="393" alt="image" src="https://github.com/user-attachments/assets/f7c2c41f-15e7-41fa-88e2-f882bf70c9c0" />

- Predicted vs. Actual price comparison plots
  <img width="1160" height="547" alt="image" src="https://github.com/user-attachments/assets/5fe3e840-18b1-482e-afa9-021a832d0997" />

- Evaluation metrics (MAE, RMSE)
  <img width="1160" height="547" alt="image" src="https://github.com/user-attachments/assets/ca32c3ac-b09a-4d61-bee5-0819280ccc5d" />

- Saved model files inside the `models/` directory  

Example structure:
```
.
├── Stock Price Prediction using LSTM.ipynb   # Main notebook
├── models/                                     # Directory for saved models
└── README.md                                   # Project documentation
```

---

## 🔧 Customization Ideas

- Experiment with different tickers (`MSFT`, `GOOG`, `TSLA`, etc.)  
- Add technical indicators (RSI, MACD, Moving Averages)  
- Tune hyperparameters: sequence length, batch size, learning rate  
- Extend the notebook to forecast multiple days ahead  

---

## 🧩 Future Enhancements

- Develop a **Streamlit** or **Gradio** dashboard for live stock predictions  
- Automate data updates and retraining  
- Explore other architectures like GRU or Transformer models  

---

## 🪪 License

This project is licensed under the **MIT License** — you’re free to use, modify, and share it with proper attribution.

---

## 🙌 Acknowledgements

- [Yahoo Finance API (`yfinance`)](https://github.com/ranaroussi/yfinance)  
- [TensorFlow](https://www.tensorflow.org/) and [Keras](https://keras.io/)  
- [Scikit-Learn](https://scikit-learn.org/)  
- [Matplotlib](https://matplotlib.org/)
