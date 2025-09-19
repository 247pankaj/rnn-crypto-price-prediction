# 📈 RNN-crypto-price-prediction

This repository contains the implementation of my **MSc Final Project (University of Hertfordshire, 2021)** on Bitcoin price prediction using Recurrent Neural Networks (RNNs), specifically LSTM and GRU models in sequential, parallel, and bidirectional architectures.

The aim was to explore deep learning approaches for predicting cryptocurrency prices and compare their effectiveness in single, two-layer, and three-layer architectures.

# 📌 Project Overview

Objective: Identify the most efficient and accurate deep learning model for short-term Bitcoin price prediction.

Techniques: LSTM, GRU, Bidirectional RNNs, Sequential & Parallel architectures.

Dataset: Bitcoin historical data from CoinMarketCap.

Frameworks: Python, Keras, TensorFlow, scikit-learn.

Key research questions included:

Do GRU models outperform LSTM models in multilayer architectures?

Does stacking layers improve prediction accuracy?

Are bidirectional RNNs more effective than standard ones?

Does increasing hidden units improve performance?

# 🗂 Dataset

The dataset consists of Bitcoin daily price data with the following features:

Date – reported date

Open – opening price

High – highest price of the day

Low – lowest price of the day

Close – closing price (target variable)

Volume – total trading volume

Market Cap – total market capitalization

Data source: CoinMarketCap Historical Data.

# ⚙️ Methodology

Data Preprocessing:

Normalization using MinMaxScaler

Train-test split (80/20)

Transformation into supervised learning format using time steps

Modeling:

Built RNN models with GRU and LSTM

Implemented in single-layer, two-layer, and three-layer setups

Explored sequential vs parallel architectures with Keras Functional API

Trained with adam optimizer and mse loss

Evaluation Metrics:

Mean Absolute Error (MAE)

Root Mean Squared Error (RMSE)

Mean Absolute Percentage Error (MAPE)

# 📊 Results

Best Model: Bidirectional GRU (2-layer, sequential) → MAPE: 5.55%

Single-layer GRU also performed strongly (MAPE: 5.78%).

LSTM models were less accurate overall, especially in deeper architectures.

Adding more than two layers (e.g., 3-layer) reduced performance.

Increasing hidden units improved accuracy but increased training time.

📌 Conclusion: GRUs outperform LSTMs, and two-layer bidirectional GRUs gave the most accurate predictions.

Run Jupyter Notebook:

jupyter notebook


Open the provided notebook (crypto_prediction.ipynb) to explore preprocessing, model building, training, and evaluation.

# 📦 Dependencies

Python 3.7+

NumPy

Pandas

Matplotlib & Seaborn

Scikit-learn

TensorFlow / Keras

Jupyter Notebook


# 🔮 Future Work

Hyperparameter tuning (optimizers, batch size, time steps)

Experiment with dropout and regularization

Try hybrid architectures (CNN-LSTM, TCN)

Extend to other cryptocurrencies (ETH, LTC, BNB, XMR)

Integrate into an automated trading bot

📖 Reference

This project was submitted as part of the MSc Data Science and Analytics program at the University of Hertfordshire (2021).
