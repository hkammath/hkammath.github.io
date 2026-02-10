---
title: "Forecasting the U.S. House Price Index: Macroeconomic & Market Signals"
date: 2025-07-17
draft: false
description: "Using Random Forest and Decision Tree models to predict U.S. home prices by analyzing GDP, CPI, and sector-specific stock performance."
tags: ["AI in Finance", "Machine Learning", "Economic Forecasting", "Python", "Random Forest", "Real Estate Analytics"]
categories: ["Data Science", "Finance"]
showTableOfContents: true
---

### Project Overview
The U.S. housing market is a cornerstone of the global economy, influenced by a complex web of macroeconomic indicators and sector-specific performance. In this collaborative project, my team and I built a predictive framework to forecast the **All-Transactions House Price Index (HPI)** by integrating traditional economic data with stock market signals.

### Tech Stack
* **Languages:** Python
* **Data Sources:** Federal Reserve Economic Data (FRED), Yahoo Finance, Kaggle
* **Machine Learning:** Scikit-Learn (Random Forest, Decision Trees)
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn

---

### The Hypothesis
We hypothesized that beyond standard economic metrics like GDP and inflation, specific stock tickers could act as leading indicators for the housing market:
* **BAC (Bank of America):** Representing the financial sector and mortgage lending health.
* **HD (Home Depot):** Reflecting consumer spending on home improvement and housing momentum.
* **NYA (NYSE Composite Index):** Serving as a broad benchmark for overall market sentiment.

### The Solution: Integrated Predictive Modeling

#### 1. Data Engineering & Feature Selection
We aggregated diverse datasets to create a comprehensive feature set:
* **Economic Indicators:** GDP, Consumer Price Index (CPI), Unemployment Rate, and Mortgage Rates.
* **Market Signals:** Historical price data for BAC, HD, and NYA.
* **Preprocessing:** Handled stationarity and multicollinearity through rigorous exploratory data analysis (EDA).

#### 2. Comparative Model Analysis
We compared the performance of single-model vs. ensemble-model approaches:
* **Decision Tree Classifier:** Used as a baseline to understand fundamental feature splits.
* **Random Forest Regressor:** Implemented as our primary model to capture non-linear relationships and reduce the variance inherent in economic data.

### Key Results & Economic Insights
* **Model Dominance:** The **Random Forest** model significantly outperformed the single Decision Tree, demonstrating higher robustness in handling the complex dynamics of the housing market.
* **Core Drivers:** Our analysis confirmed that **GDP, CPI, and Mortgage Rates** remain the most powerful standalone predictors of home prices.
* **The "Ticker" Signal:** While sector-specific stocks (BAC and HD) provided depth and sentiment context, they functioned best as supplementary signals rather than primary drivers.
* **Visualizing the Market:** Developed detailed correlation heatmaps and feature importance plots to illustrate the hierarchy of factors influencing the HPI.

---

### Conclusion
This project underscores the value of ensemble learning in financial forecasting. By bridging the gap between broad macroeconomic trends and specific market assets, we developed a tool capable of providing early signals for shifts in the U.S. housing market, a critical asset for investors and policy-makers alike.

> [View Python Notebook](/uploads/us_housing_python_notebook.ipynb)