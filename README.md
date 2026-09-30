# 💰 Dynamic Pricing Engine for E-commerce

An AI-based dynamic pricing prototype that uses machine learning to estimate a recommended product price from demand, inventory, competitor, seasonal, and transaction-related information.

## 📌 Project Overview

Dynamic pricing systems can adjust product prices based on changing market and business conditions.

This project implements an educational MVP using synthetically generated e-commerce data and an XGBoost regression model.

The application provides:

- XGBoost-based price prediction
- Feature engineering from e-commerce signals
- Demand-related features
- Inventory information
- Competitor pricing information
- Seasonal features
- Interactive Streamlit dashboard
- Recommended price prediction

## 🎯 Objective

Build a machine learning prototype that analyzes e-commerce conditions and predicts a suitable product price.

The internship guide includes advanced requirements such as demand forecasting, price elasticity, revenue optimization, competitor pricing, FastAPI, Kafka, Redis, cloud deployment, and monitoring.

This MVP focuses on the core machine-learning pricing prediction pipeline and interactive application.

## 📊 Data and Features

The prototype uses synthetically generated e-commerce data.

The training pipeline incorporates signals such as:

- Product price
- Demand / sales-related information
- Inventory level
- Competitor price
- Seasonal information
- Click and order activity

The synthetic dataset is generated during model training for reproducibility.

## 🤖 Machine Learning Approach

The project uses **XGBoost Regression** to predict a recommended product price.

### Training pipeline

1. Generate synthetic e-commerce data
2. Prepare and engineer input features
3. Split the dataset into training and validation data
4. Train the XGBoost regression model
5. Generate price predictions
6. Evaluate regression performance
7. Save the trained model
8. Load the model in the Streamlit application

## 📈 Model Evaluation

The regression model is evaluated using:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

These metrics are used to measure the difference between predicted and target prices.

## 🖥️ Streamlit Application

The project includes an interactive Streamlit interface.

The user can provide product and market-related inputs and receive a predicted/recommended price.

The application demonstrates how a trained machine-learning model can be connected to an interactive pricing interface.

## 📂 Project Structure

```text
project2-dynamic-pricing/
│
├── artifacts/
│   └── pricing_model.joblib
│
├── app.py
├── train.py
├── requirements.txt
├── README.md
├── .gitignore
└── screenshots/
```

---

## ⚙️ Installation

Create and activate a virtual environment:

### Windows
python -m venv .venv
.venv\Scripts\activate

Install the dependencies:

pip install -r requirements.txt

## 🚂 Train the Model

Run:

python train.py

The trained model is saved as:

artifacts/pricing_model.joblib

## 🚀 Run the Application

Start the Streamlit application:

streamlit run app.py

The application will open in the browser and provide an interactive pricing interface.

## 📁 Dataset

This prototype uses synthetically generated e-commerce data.

The dataset is intended for educational and demonstration purposes and is not representative of real-world commercial pricing data.

## ⚠️ Limitations

This is an educational MVP implementation.

Current limitations include:

- Synthetic training data is used.
- The model has not been validated using real-world e-commerce data.
- A dedicated price-elasticity estimation module is not implemented.
- A full revenue-optimization engine is not implemented.
- Real-time competitor APIs are not integrated.
- Kafka-based event streaming is not implemented.
- Redis-based caching is not implemented.
- A FastAPI inference service is not included.
- Cloud deployment is not included in the current prototype.
- Production monitoring and automated model retraining are not implemented.

Therefore, the predicted prices should be treated as prototype outputs rather than production pricing recommendations.

## 🔮 Future Improvements

Possible improvements include:

Training with real e-commerce datasets
Price elasticity estimation
Revenue optimization
Real-time competitor price integration
FastAPI inference endpoint
Kafka event streaming
Redis caching
Docker containerization
AWS deployment
Monitoring and logging
Model drift detection
Automated model retraining
🛠️ Technology Stack
Python
Pandas
NumPy
Scikit-learn
XGBoost
Joblib
Streamlit

---
## ✅ Project Status

Completed — Internship Prototype

The machine-learning model has been trained successfully, the trained model artifact has been generated, and the Streamlit application has been tested locally.