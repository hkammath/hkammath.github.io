---
title: "Predicting Academic Success: A Machine Learning Approach"
date: 2025-04-12
draft: false
description: "Developing a multi-class classification model to predict student dropout and academic success using the UCI Student Dropout dataset."
tags: ["Machine Learning", "Python", "Predictive Analytics", "Scikit-Learn", "Data Engineering"]
categories: ["Data Science"]
showTableOfContents: true
---

### Project Overview
The ability to predict whether a student will graduate or drop out is a critical challenge for educational institutions. This project leverages machine learning to analyze demographic, socio-economic, and academic data to identify students at risk, allowing for proactive administrative intervention.

### Tech Stack
- **Languages:** Python
- **Libraries:** Pandas, NumPy, Scikit-Learn, Matplotlib, Seaborn
- **Algorithms:** Random Forest, Support Vector Machines (SVM), K-Nearest Neighbors (KNN), Logistic Regression

---

### The Problem
Educational institutions struggle with high dropout rates which impact both funding and institutional reputation. The goal was to build a robust classification engine capable of predicting three outcomes: **Dropout, Enrolled, or Graduate**, based on data available at the time of student enrollment and after the first year.

### The Solution
The approach followed a rigorous data science pipeline, ensuring the model was not only accurate but also generalizable.

#### 1. Data Engineering & Preprocessing
- **Data Cleaning:** Cleaned feature headers and validated 4,424 instances across 37 features.
- **Outlier Mitigation:** Applied the **Interquartile Range (IQR)** method to the "Admission Grade" feature to reduce noise in distance-based models.
- **Feature Transformation:** - Scaled numerical features using `StandardScaler` to optimize performance for SVM and KNN.
    - Implemented **One-Hot Encoding** for categorical variables to ensure mathematical compatibility.

#### 2. Exploratory Data Analysis (EDA)
Before modeling, I explored key drivers of student success:
- **Admission Grades:** Higher initial grades showed a strong correlation with graduation rates.
- **Age at Enrollment:** Visualized age distributions to understand non-traditional student trends.
- **Class Balance:** Identified a majority class of 'Graduates', which informed the use of **F1-Score** and **Precision-Recall** metrics over simple accuracy.

#### 3. Model Comparison
I evaluated multiple classification algorithms to identify the optimal balance between bias and variance:
- **Logistic Regression & Decision Trees:** Used as baseline models.
- **KNN & SVM:** Analyzed for their ability to handle high-dimensional feature spaces.
- **Random Forest:** Selected as the final model due to its ability to capture complex feature interactions and its inherent resistance to overfitting.

### Key Results & Insights
- **Performance Boost:** Feature scaling and outlier removal significantly improved the accuracy of distance-dependent algorithms.
- **Top Predictor:** Academic performance in the first and second semesters emerged as the most significant predictor of the final outcome.
- **Actionable Insight:** The model successfully identified key socio-economic indicators (like scholarship status and parental qualifications) that correlate with student persistence.

---

### Conclusion
This project demonstrates the power of machine learning in supporting informed decision-making in the education sector. By deploying the **Random Forest** model, institutions can move from reactive reporting to proactive student support.

> [View Python Notebook](/uploads/intro_to_ml_python_notebook.ipynb)