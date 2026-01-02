# Economic Forecasting with Multiple Regression in Python

A hands-on Python example showing how to build a **basic, interpretable economic forecast** using **multiple regression** and real-world macroeconomic data from the Federal Reserve (FRED).

This repository accompanies the blog post:

**“How to Create Your Own Basic Economic Forecast Using Multiple Regression in Python”**

![Python](https://img.shields.io/badge/python-3.9%2B-blue)
![Jupyter Notebook](https://img.shields.io/badge/jupyter-notebook-orange)
![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)

---

## 📌 Overview

Economic forecasts don’t need to be complicated to be useful.

This project demonstrates how to:
- Use **multiple regression** as a *structural* econometric model  
- Model **consumer spending** as a function of income, interest rates, and inflation  
- Work with **real, publicly available data**  
- Turn a regression model into a **simple, scenario-based forecast**

The goal is not perfect prediction.  
The goal is **clarity, intuition, and better decision-making**.

---

## 📊 What This Project Does

- Pulls monthly macroeconomic data directly from **FRED**
- Cleans and transforms the data for regression
- Fits a multiple regression model using Python
- Evaluates out-of-sample performance
- Generates simple forecasts under different economic assumptions

---

## 🧠 Model Concept

Conceptually, the model estimates:
Consumer Spending = f(Income, Interest Rates, Inflation)

In practice, the notebook models **growth in real consumer spending** using:
- Real disposable personal income growth
- Inflation (year-over-year)
- The federal funds rate

Robust (Newey–West / HAC) standard errors are used to account for common issues in macroeconomic time series data.

---

## 📁 Repository Structure

├── basic_economic_forecast_using_multiple_regression.ipynb
├── README.md
├── LICENSE
└── .gitignore

---

## ▶️ How to Run the Notebook

### Option 1: Run Locally

1. Clone the repository:
   ```bash
   git clone https://github.com/joedom99/economic-forecasting-multiple-regression-python.git
   cd economic-forecasting-multiple-regression-python
2. Install dependencies
3. Launch Jupyter notebook
4. Open: basic_economic_forecast_using_multiple_regression.ipynb

### Option 2: Run in Google Colab

You can upload the notebook directly to Google Colab and run it without any local setup.

## 📈 Data Sources

All data is sourced from the Federal Reserve Bank of St. Louis (FRED):
	•	Personal Consumption Expenditures (PCE)
	•	Disposable Personal Income (DPI)
	•	Consumer Price Index (CPI)
	•	Federal Funds Effective Rate

These series are widely used in professional economic analysis and are updated regularly.

## ⚠️ Important Notes & Limitations
	•	This is a structural regression model, not a pure time-series model
	•	Forecasts require assumptions about future inputs
	•	The model reflects average economic behavior, not distributional differences
	•	Structural breaks and shocks (e.g., pandemics, policy changes) are not explicitly modeled

This project is intentionally simple and educational.

## 🔭 Possible Extensions
	•	Forecast the independent variables using ARIMA or SARIMA
	•	Combine regression and time series (dynamic regression / ARIMAX)
	•	Add lagged variables or additional predictors
	•	Segment the model to explore uneven economic effects

## 📜 License

This project is licensed under the MIT License.
See the LICENSE￼ file for details.

## 🙌 Acknowledgments
	•	Federal Reserve Bank of St. Louis (FRED) for open economic data
	•	The Python open-source ecosystem for making applied econometrics accessible
