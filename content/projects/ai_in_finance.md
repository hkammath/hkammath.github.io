---
title: "Cryptocurrency Dynamics: Predictive Modeling & Cluster Analysis"
date: 2025-07-20
draft: false
description: "Applying Random Forest classification and K-Means clustering to analyze volatility and predict price movements in the top 10 cryptocurrencies."
tags: ["AI in Finance", "Machine Learning", "Python", "Clustering", "Financial Modeling", "Cryptocurrency"]
categories: ["Data Science"]
showTableOfContents: true
---

### Project Overview
The cryptocurrency market is characterized by extreme volatility and complex price dynamics. In this project, I explored price behavior for the top 10 digital assets by market capitalization, using machine learning to classify price movements and group assets based on their risk-return profiles.

### Tech Stack
* **Languages:** Python
* **Libraries:** Scikit-Learn, NumPy, Pandas, Plotly
* **Supervised Learning:** Random Forest, Decision Tree Classifiers
* **Unsupervised Learning:** K-Means Clustering

---

### The Problem
Traditional financial models often struggle with the non-linear nature of crypto assets. The goal was to determine if technical indicators (like momentum and volatility) could accurately predict short-term price direction for Bitcoin (BTC) and to identify underlying market structures through clustering.

### The Solution: A Dual-Model Framework

#### 1. Supervised Classification (Predicting Market Direction)
I built a model to classify whether Bitcoin's price would rise or fall the following day:
* **Feature Engineering:** Developed domain-specific features including 3-day and 7-day rolling volatility, momentum indicators (open-close spreads), and lagged returns.
* **Model Selection:** Compared **Decision Trees** and **Random Forest Classifiers**.
* **Optimization:** Used feature importance analysis to identify that short-term momentum and volatility were the strongest predictors of price movement.

#### 2. Unsupervised Clustering (Risk-Return Grouping)
To understand asset relationships, I applied **K-Means Clustering** to the broader market:
* **Standardization:** Normalized features to ensure equal weighting in distance calculations.
* **Asset Segregation:** The model successfully identified three distinct "asset classes" within the top 10 coins:
    * **Stable Leaders:** Low-volatility, mature assets (e.g., BTC, ETH).
    * **High-Growth Candidates:** Moderate volatility with strong risk-adjusted returns.
    * **Speculative Outliers:** High-volatility assets with extreme return potential.

### Key Results & Financial Insights
* **Predictive Accuracy:** The Random Forest model provided high precision in predicting price rises, outperforming baseline measures.
* **Portfolio Diversification:** The clustering analysis provided a scalable framework for grouping assets based on risk preference rather than just market cap.
* **Visualizing Risk:** Developed interactive 2D scatterplots (Return vs. Volatility) using **Plotly** to interpret cluster groupings and asset dynamics in real-time.

---

### Conclusion
This project demonstrates how combining financial domain knowledge with classical machine learning can yield actionable insights in rapidly evolving markets. By integrating technical indicators with robust clustering, I developed a toolset capable of identifying both market-wide trends and specific asset-level opportunities.

> [Download the Full Technical Report](/uploads/ai_in_finance_business_report.pdf)

> [View Python Notebook](/uploads/ai_in_finance_python_notebook.ipynb)