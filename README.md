# Economic Forecasting with Multiple Regression in Python

A hands-on Python example showing how to build a **basic, interpretable economic forecast** using **multiple regression** and real-world macroeconomic data from the Federal Reserve (FRED).

This repository accompanies the blog post:

**“How to Create Your Own Basic Economic Forecast Using Multiple Regression in Python”**

![Python](https://img.shields.io/badge/python-3.9%2B-blue)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1VqZmMV2DRFsTw7Ed42U9qfBN0lMiCevm?usp=sharing)
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

Conceptually, the model estimates the "tug-of-war" between five economic forces: **Consumer Spending = f(Income, Sentiment, Inflation, Rates, Unemployment)**

In practice, the notebook forecasts Real Personal Consumption Expenditures (PCE) using:

* Real Disposable Personal Income: "The Fuel" (Positive Driver)
* Consumer Sentiment (UMCSENT): "The Psychology" (Positive Driver)
* Inflation (CPI): "The Friction" (Negative Drag)
* Federal Funds Rate: "The Brake" (Negative Drag)
* Unemployment Rate: "The Fear Factor" (Negative Drag)

Robust (Newey–West / HAC) standard errors are used to account for common issues in macroeconomic time series data.

---

## 📁 Repository Files

* (Main forecast notebook) basic_economic_forecast_using_multiple_regression.ipynb
* (OPTIONAL notebook to create article plots) Optional_Economic_Forecast_Plots_for_the_article.ipynb
* (OPTIONAL saved dataset used for article) my_economic_forecast_data.csv
* README.md
* LICENSE

---

## 👨🏻‍💻 Reproducibility & Data Integrity
This analysis was originally generated on **January 3, 2026.**

Because this project relies on live economic data from the Federal Reserve (FRED), results generated in the future may differ slightly due to official government data revisions and updates.

To ensure reproducibility, I have included a "Time Capsule" of the raw data used for the article.

* **Live Mode (Default**): The notebook is set to pull the most current data from the FRED API. This ensures the forecast uses the latest available information.
* **Static Mode (Reproducible)**: To reproduce the exact results found in the article, you can load the provided snapshot file (my_economic_forecast_data.csv) instead of querying the API.

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
