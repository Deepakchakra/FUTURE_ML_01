📊 Sales Demand Forecast & Prediction System

An End-to-End Machine Learning project that predicts retail store sales and forecasts future demand using historical business data.

The system uses multiple machine learning models to analyze past sales patterns and generate real-time predictions and 30-day forecasts through an interactive Streamlit dashboard.

🚀 Live Demo

Try the deployed application:

👉 https://futureml01-4ktpobgypu384nsffaaxat.streamlit.app/

📌 Project Overview

Sales forecasting is essential for businesses to optimize inventory, manage supply chains, and improve revenue planning.

This project builds a complete ML pipeline that:

Processes historical store sales data

Engineers time-series features

Trains multiple machine learning models

Selects the best model

Deploys the model with a real-time dashboard

The final system allows users to:

Predict sales for a given store and date

Forecast the next 30 days of sales

Visualize important factors affecting sales

🎯 Problem Statement

Businesses often struggle to estimate future demand accurately.
Incorrect forecasts can lead to:

Overstocking

Inventory shortages

Revenue loss

Inefficient supply chain management

The goal of this project is to build a machine learning system that predicts future store sales using historical sales data and business features.

📂 Dataset

The dataset used in this project contains historical retail store data including:

Store ID

Date

Promotion information

Holiday indicators

Store type

Assortment type

Historical sales

Competition distance

Customer data

These features are used to train machine learning models to predict future sales.

🧠 Machine Learning Models Used

Multiple models were trained and compared:

Random Forest

XGBoost

LightGBM

Prophet (Time-Series Model)

The best performing model was selected based on evaluation metrics.

⚙️ Machine Learning Pipeline

The project follows a complete ML pipeline:

1️⃣ Data Collection
2️⃣ Data Cleaning & Preprocessing
3️⃣ Feature Engineering
4️⃣ Model Training
5️⃣ Model Evaluation
6️⃣ Model Selection
7️⃣ Forecast Generation
8️⃣ Dashboard Deployment

📊 Features of the Dashboard

The Streamlit dashboard provides three main functionalities:

🔴 Real-Time Prediction

Predict store sales based on user input such as:

Store ID

Promotion status

Holiday indicators

Previous sales data

Store type and assortment

📈 30-Day Sales Forecast

Generate predicted sales for the next 30 days and visualize:

Forecast trend

Average predicted sales

Target revenue line

Maximum and minimum predicted sales

📊 Feature Importance

Displays the most important factors influencing sales predictions.

📁 Project Structure
Sales_Demand_Forecast
│
├── dashboard
│   └── app.py
│
├── src
│   ├── data_preprocessing.py
│   ├── feature_engineering.py
│   ├── forecasting.py
│   ├── model_random_forest.py
│   ├── model_xgboost.py
│   ├── model_lightgbm.py
│   └── model_prophet.py
│
├── models
│   ├── xgboost.pkl
│   └── xgb_feature_columns.pkl
│
├── reports
│
├── main.py
├── requirements.txt
└── README.md

📊 Model Evaluation

Models were evaluated using:

MAE (Mean Absolute Error)
RMSE (Root Mean Squared Error)
R² Score

Example result:

Model	R² Score
Random Forest	0.81
XGBoost	0.83 (Best)
LightGBM	0.79
Prophet	0.19

XGBoost was selected as the final model.

💻 Technologies Used

Programming Language

Python

Libraries

Pandas

NumPy

Scikit-learn

XGBoost

LightGBM

Prophet

Matplotlib

Framework

Streamlit

Deployment

Streamlit Cloud

▶️ How to Run the Project Locally

Clone the repository:

git clone https://github.com/Deepakchakra/FUTURE_ML_01.git

Go to project folder:

cd FUTURE_ML_01

Install dependencies:

pip install -r requirements.txt

Run the dashboard:

streamlit run dashboard/app.py
