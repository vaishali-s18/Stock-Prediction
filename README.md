# Stock Price Prediction 

This project is a **Stock Price Prediction web application** built using Python, Machine Learning, and Deep Learning.

The main idea behind this project is to use historical stock market data and learn the patterns in the data to predict future stock prices. Since stock prices can change due to many different factors, predicting them accurately is difficult. This project is mainly created to understand how **time-series data and LSTM models** can be used for stock price prediction.

The project also has a simple **Streamlit interface** where users can select a stock and view its historical data and predictions.

---

## Features

- Get historical stock data using Yahoo Finance
- View stock price charts
- Preprocess and normalize stock data
- Use an LSTM model for prediction
- Compare actual and predicted prices
- Display results through a Streamlit application
- Simple and easy-to-use interface

---

## Technologies Used

- **Python**
- **NumPy** – for numerical calculations
- **Pandas** – for handling and analyzing data
- **YFinance** – for getting stock market data
- **Matplotlib** – for creating graphs
- **Scikit-learn** – for data preprocessing and evaluation
- **TensorFlow / Keras** – for building the LSTM model
- **Streamlit** – for creating the web application

---

## How the Project Works

The basic flow of the project is:

```text
Select Stock
     ↓
Get Historical Data
     ↓
Clean and Prepare Data
     ↓
Normalize the Data
     ↓
Create Training Sequences
     ↓
Train / Load LSTM Model
     ↓
Predict Stock Prices
     ↓
Display Graphs and Results
```

### 1. Getting Stock Data

The project uses **YFinance** to collect historical stock market data.

The data can include:

- Open price
- High price
- Low price
- Closing price
- Volume

### 2. Data Preprocessing

After getting the data, it is cleaned and prepared before giving it to the model.

The stock prices are scaled using `MinMaxScaler` so that the values are in a suitable range for the neural network.

### 3. Creating Sequences

Since stock prices are time-series data, previous prices are used to predict the next price.

For example:

```text
Previous Prices
[100, 102, 101, 105, 107]

        ↓

LSTM Model

        ↓

Predicted Price
108
```

### 4. LSTM Model

An **LSTM (Long Short-Term Memory)** neural network is used because it works well with sequential data.

The model learns patterns from the historical stock prices and uses those patterns to generate predictions.

### 5. Showing the Results

The predicted values are displayed using graphs so that the actual and predicted prices can be compared easily.

---

## Project Structure

```text
Stock-Price-Prediction/
│
├── app.py
├── README.md
├── requirements.txt
│
└── ...
```

The main application is present in `app.py`.

---

## Installation

### Clone the repository

```bash
git clone https://github.com/your-username/Stock-Price-Prediction.git
```

### Go to the project folder

```bash
cd Stock-Price-Prediction
```

### Create a virtual environment

```bash
python -m venv .venv
```

Activate it on Windows:

```bash
.venv\Scripts\activate
```

### Install the required libraries

```bash
pip install -r requirements.txt
```

If you don't have a `requirements.txt` file, you can install the libraries using:

```bash
pip install numpy pandas yfinance tensorflow keras streamlit matplotlib scikit-learn
```

---

## Run the Project

After installing the dependencies, run:

```bash
python -m streamlit run app.py
```

The application will open in your browser.

Usually, it will be available at:

```text
http://localhost:8501
```

---

## Screenshots

You can add screenshots of the application here.

For example:

```markdown
![Home Page](screenshots/home.png)

![Stock Chart](screenshots/chart.png)

![Prediction](screenshots/prediction.png)
```

---

## What I Learned From This Project

While working on this project, I got practical experience with:

- Working with real-world stock market data
- Data cleaning and preprocessing
- Using APIs to collect data
- Data visualization
- Time-series data
- LSTM neural networks
- Using Python libraries for machine learning
- Building a simple application using Streamlit

---

## Future Improvements

There are several things that can be added to this project in the future, such as:

- Adding more technical indicators
- Comparing different machine learning models
- Trying GRU or Transformer-based models
- Adding news sentiment analysis
- Adding more visualization options
- Deploying the application online
- Adding real-time stock updates

---

## Disclaimer

This project is made for **learning and educational purposes**.

Stock prices are affected by many factors and can be unpredictable. The predictions from this project should not be treated as financial advice or as a guarantee of future stock prices.

---

## Author

**Vaishali**

B.Tech Computer Science Engineering
