# 📈 Stock Prediction using Time Series Analysis (Deep LSTM)

A **Time Series Stock Price Prediction** project using **Apple (AAPL)** historical data.  
This notebook downloads real stock data using **Yahoo Finance**, performs preprocessing + scaling, creates **lag features**, trains a **Deep LSTM neural network**, and evaluates predictions using regression metrics.

---

## ✅ Project Highlights

- 📥 Fetch real-time stock data using **yFinance**
- 🧹 Data preprocessing and **Min-Max Scaling**
- ⏳ Lag feature creation (Past **15 days**)
- 🧠 Deep Learning Model: **LSTM (Long Short-Term Memory)**
- 📊 Performance evaluation with **MAE, RMSE, R²**
- 📉 Actual vs Predicted visualization

---

## 🧾 Dataset Used

This project uses stock data from **Yahoo Finance**:

- Stock: **Apple Inc. (AAPL)**
- Duration: **Last 6 Years**
- Features include: `Open`, `High`, `Low`, `Close`, `Adj Close`, `Volume`

Source: Yahoo Finance via `yfinance`

---

## 🛠️ Technologies Used

- **Python**
- **NumPy**
- **Pandas**
- **Matplotlib**
- **yFinance**
- **Scikit-learn**
- **TensorFlow / Keras**

---

## 🧠 Workflow (Steps in Notebook)

### ✅ Step 1: Import Libraries
All required libraries are imported such as NumPy, Pandas, TensorFlow, sklearn, etc.

### ✅ Step 2: Download Stock Data
Apple stock data is fetched using:

- `yfinance.download()`

### ✅ Step 3: Data Scaling
Stock prices are normalized using:

- `MinMaxScaler`

### ✅ Step 4: Create Lag Features (Past 15 Days)
A supervised learning dataset is built where the model predicts the next value based on the last **15 days**.

### ✅ Step 5: Train-Test Split
The dataset is split into:

- Training Data
- Testing Data

### ✅ Step 6: Build Deep LSTM Model
A deep LSTM model is created using Keras:

- LSTM layers
- Dense output layer
- Adam optimizer

### ✅ Step 7: Training the Model
Model is trained on training data with a chosen number of epochs and batch size.

### ✅ Step 8: Predictions & Evaluation
Predictions are made and evaluated using:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

### ✅ Step 9: Visualization
Graph plotted for:

- Actual vs Predicted stock prices

---

## 📌 How to Run the Project

### ✅ 1. Clone the Repository
```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```
### ✅ 2. Install Required Libraries
```bash
pip install numpy pandas matplotlib yfinance scikit-learn tensorflow
```
### ✅ 3. Run the Notebook

Open and run in Jupyter Notebook / VS Code:
```bash
jupyter notebook Stock-Prediction-Time-Series-Analysis.ipynb
```
## 📊 Model Evaluation Metrics

The notebook evaluates prediction performance using:

- MAE → Measures average error

- RMSE → Penalizes larger errors more

- R² Score → Measures overall goodness of fit

## 📷 Output Example

### ✅ Graph Output:

- Blue line = Actual Price

- Red line = Predicted Price

(Your notebook generates this automatically)

# 👨‍💻 Author

## Ajay Singh
### 📌 Project: Stock Prediction using Deep Learning (LSTM)
