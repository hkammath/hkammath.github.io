---
title: "Precision Scouting: 2025 NFL Draft Prediction Model"
date: 2025-06-11
draft: false
description: "Using machine learning to drive the New York Jets' 2025 draft strategy, optimizing roster needs with high-precision prospect modeling."
tags: ["Machine Learning", "Sports Analytics", "Python", "Predictive Modeling", "NFL Draft"]
categories: ["Data Science"]
showTableOfContents: true
---

### Project Overview
In a multi-session simulation of the 2025 NFL Draft, I served as the Lead Data Analyst for the **New York Jets**. The objective was to break a 14-season playoff drought by using machine learning to identify high-value prospects who fit the team's specific positional needs and scheme requirements.

### Tech Stack
* **Languages:** Python
* **Libraries:** Scikit-Learn, Pandas, NumPy, Matplotlib
* **Modeling:** Gradient Boosting, Random Forest, Logistic Regression
* **Strategy:** Financial Constraint Analysis, Competitive Pressure Modeling

---

### The Problem
The New York Jets entered the 2025 off-season with significant gaps in the Offensive Line, Wide Receiver, and Quarterback rooms. The challenge was to move beyond traditional scouting by using data to predict a prospect's "Success Probability" while navigating financial constraints and the competitive draft environment.

### The Solution: The "Front Office" Pipeline

#### 1. Roster Gap Analysis
I started by quantifying the "Gap" between the Jets' current performance (PFF Grades) and the AFC average. This data-driven audit prioritized our draft board:
* **Primary Needs:** Offensive Line (-16.3 Gap) and Quarterback (-16.4 Gap).
* **Secondary Needs:** Wide Receivers (-11.7 Gap).

#### 2. Machine Learning Model Development
I developed a classification model to rank prospects based on historical performance data and physical traits:
* **Feature Engineering:** Integrated collegiate stats, combine results, and PFF advanced metrics.
* **Model Selection:** Compared several algorithms, focusing on **Precision** to avoid "bust" picks in the early rounds.
* **Ranking System:** Generated a proprietary "Model Ranking" for every position, allowing the GM to see how a prospect stacked up against their peers in real-time.

#### 3. Executing the Draft Strategy
Using the model's output, we executed a strategy focused on "Winning Now":
* **Round 1:** Targeted elite protection for the offensive line based on top-tier model rankings.
* **Mid-Rounds:** Identified "Sleepers" like **Jordan Burch (DE)** and **Quandarrius Robinson (LB)**, who the model ranked significantly higher than their projected draft position due to their explosive physical traits.

### Key Results & Impact
* **Strategy vs. Intuition:** The model successfully identified high-upside players in the 4th round who filled critical depth roles behind veterans like C.J. Mosley.
* **Balanced Roster:** Successfully addressed all three primary "Weakness Gaps" identified during the pre-draft phase.
* **Competitive Edge:** The simulation demonstrated that integrating ML into the "War Room" allows for faster, more objective decision-making when elite prospects are taken off the board.

---

### Conclusion
This project highlights the intersection of sports business acumen and predictive analytics. By quantifying talent and roster needs, I helped transform the Jets' draft from a game of chance into a precision-driven operation aimed at ending the longest playoff drought in the league.

> [View Python Notebook](/uploads/nfl_draft_python_notebook.ipynb)