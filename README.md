# 🌦 Weather Prediction using LSTM and ARIMA

## 📌 Overview
This project implements a **hybrid weather prediction model** combining:
- **LSTM (Long Short-Term Memory)** for capturing short-term, high-frequency patterns using hourly data.
- **ARIMA (AutoRegressive Integrated Moving Average)** for modeling long-term trends using monthly aggregated data.

The goal was to improve accuracy in forecasting temperature values by leveraging the strengths of both deep learning and statistical time-series approaches.

---

## 🗂 Project Structure
├── Weather Prediction using LSTM and ARIMA.ipynb # Jupyter notebook with full workflow

├── README.md # Project documentation

├── requirements.txt # List of dependencies

└── dataset/ # Weather dataset (not included, see below)


---

## 📊 Dataset
- **Input**: Hourly weather data (`weather_data_1hr.csv`).
- **Features**: Date, Time, Temperature, and other meteorological attributes.
- **Preprocessing**:
  - Merged date and time columns into a single `datetime` feature.
  - Normalized values using `MinMaxScaler`.
  - Prepared data for both **hourly (LSTM)** and **monthly aggregated (ARIMA)** modeling.

⚠️ *Note*: The dataset used in this project was **purchased from a third-party website**. Due to licensing and ownership considerations, it may not be freely redistributed.  

---

## ⚙️ Installation
Clone this repository:

git clone https://github.com/Vedant2606/Weather_Forecasting_New_Zealand-LSTM_ARIMA.git

## Create and activate a virtual environment:

python -m venv venv
venv\Scripts\activate


## Install required dependencies:

pip install -r requirements.txt

## 🚀 Usage

Run the Jupyter notebook to reproduce the workflow:

jupyter notebook "Weather Prediction using LSTM and ARIMA.ipynb"

Steps inside the notebook:

Data Preprocessing – clean and transform raw weather data.

Exploratory Data Analysis (EDA) – visualize seasonal trends and distributions.

Model Training – fit both ARIMA and LSTM models.

Hybrid Modeling – combined predictions for improved accuracy.

Evaluation – compared models using RMSE and other metrics.

## 📈 Results

ARIMA: Effective in modeling long-term, low-frequency variations.

LSTM: Captures hourly fluctuations and short-term dependencies.

Hybrid Model: Outperformed individual models in RMSE and trend forecasting.

## 🔮 Future Improvements

Experiment with GRU or Transformer-based architectures.

Extend dataset with humidity, wind speed, and precipitation.

Deploy model as a REST API or integrate into a dashboard.
