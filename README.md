# 🚗 Car Price Prediction — Multiple Linear Regression

A machine learning project that predicts the **market price of second-hand cars** using Multiple Linear Regression, built with Python and scikit-learn.

## 📌 Problem Statement
Used-car pricing is subjective and inconsistent. This project builds a data-driven model that estimates a fair market price based on key vehicle attributes — useful for buyers, sellers, and dealerships.

## 📦 Dataset
The dataset contains real-world used-car listings with the following features:

| Feature | Description |
|---|---|
| `Brand` | Car manufacturer (Audi, BMW, Toyota, etc.) |
| `Body` | Body style (sedan, hatch, crossover, etc.) |
| `Mileage` | Total kilometres driven |
| `EngineV` | Engine displacement in litres |
| `Engine Type` | Fuel type (Diesel, Petrol, Gas) |
| `Registration` | Valid registration status |
| `Year` | Year of manufacture |
| `Price` | Selling price in USD *(target)* |

## 🔧 Methodology

1. **Data Cleaning** — dropped irrelevant columns, handled missing values, removed outliers
2. **EDA** — distribution plots and scatter plots for all continuous features
3. **OLS Assumption Checks** — linearity verified via scatter plots; multicollinearity checked using VIF
4. **Feature Engineering** — log-transformed target variable; one-hot encoded categorical features
5. **Modelling** — StandardScaler + LinearRegression on an 80/20 train/test split
6. **Evaluation** — R², residuals distribution, and percentage error on the test set

## 📊 Results

| Metric | Value |
|---|---|
| R² (Training) | ~0.75 |
| Target Transform | log(Price) |
| Features Used | 17 (after encoding) |

## 🛠️ Tech Stack
`Python` · `scikit-learn` · `pandas` · `NumPy` · `Matplotlib` · `Seaborn` · `statsmodels`

## 🚀 Getting Started

```bash
git clone https://github.com/your-username/Car_Price_Prediction.git
cd Car_Price_Prediction
pip install -r requirements.txt
jupyter notebook car_price_prediction.ipynb
```

## 📁 Project Structure
Car_Price_Prediction/
├── Datasets/
│   └── 1.04.+Real-life+example.csv
├── car_price_prediction.ipynb
├── requirements.txt
└── README.md

## 👤 Author
**Mangaliso Maduna** — [Portfolio](https://mangaliso-maduna.github.io/portfolio/) · [LinkedIn](https://www.linkedin.com/in/mangalisom/)
