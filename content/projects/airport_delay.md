---
title: "Aviation Analytics: Predicting Delays & Forecasting Growth at CLT"
date: 2025-06-18
draft: false
description: "Implementing Random Forest and XGBoost to predict flight delays and forecasting passenger traffic through 2026 for Charlotte Douglas International Airport."
tags: ["Machine Learning", "Forecasting", "Python", "XGBoost", "Time Series", "Predictive Modeling"]
categories: ["Data Science"]
showTableOfContents: true
---

### Project Overview
Charlotte Douglas International Airport (CLT) faces increasing operational pressure from passenger growth and weather disruptions. This project delivers two critical data-driven tools: a classification model to predict flight delays ($\geq$ 15 minutes) and a forecasting model to project passenger traffic through mid-2026.

### Tech Stack
* **Languages:** Python
* **Machine Learning:** Scikit-Learn (Random Forest, Decision Trees), XGBoost
* **Deep Learning:** TensorFlow/Keras (Class weights for imbalanced data)
* **Analysis:** Time Series Forecasting, Predictive Modeling

---

### The Problem
Operational bottlenecks and revenue loss occur when airports cannot proactively manage delays or anticipate passenger surges. The goal was to translate raw flight data into actionable strategies for staffing, gate assignments, and vendor coordination at one of the busiest hubs in the U.S.

### The Solution: A Two-Pronged Approach

#### 1. Predictive Delay Modeling
I evaluated multiple classification algorithms to identify the best-performing model for predicting departure delays:
* **Algorithm Selection:** Compared **Random Forest**, **XGBoost**, and **Decision Trees**.
* **Handling Imbalance:** Utilized **Keras class weights** during training to ensure the model accurately identified the minority "delayed" class.
* **Feature Engineering:** Analyzed delay drivers including marketing carriers, day of the week, and specific hours of departure.

#### 2. Passenger Traffic Forecasting
Beyond daily operations, I built a forecasting model to predict monthly passenger volumes from June 2025 through May 2026. This allows airport leadership to plan long-term infrastructure and resource allocation effectively.

### Key Results & Strategic Insights
* **Operational Hotspots:** Identified that delay rates fluctuate significantly based on the hour of departure and specific marketing carriers.
* **Data-Driven Dashboards:** Developed visualizations tracking delay distributions and top 10 destination delay rates.
* **Actionable Recommendations:** 
    * **Staffing:** Optimized security and gate staffing during forecasted peak passenger windows.
    * **Vendor Coordination:** Advised commercial vendors on inventory management based on departure delay probabilities.
    * **Infrastructure:** Provided data to support long-term planning for gate expansion and terminal flow.

---

### Conclusion
By combining classification and forecasting, this project moves airport management from reactive reporting to proactive decision-making. The models provide a clear framework for protecting revenue and improving the passenger experience at CLT.

> [Download the Full Technical Report](/uploads/airport_delay_business_report.pdf)

> [View Python Notebook](/uploads/airport_delay_python_notebook.ipynb)