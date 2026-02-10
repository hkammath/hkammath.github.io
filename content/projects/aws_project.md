---
title: "Carrier On-Time Performance: Big Data Analytics with AWS"
date: 2024-12-04
draft: false
description: "Building a cloud-native ETL pipeline to analyze 10.4M+ flight records and optimize travel schedules."
tags: ["AWS", "SQL", "Big Data", "Data Engineering", "Athena", "Glue"]
categories: ["Data Engineering"]
showTableOfContents: true
---

### Project Overview
This project involved the processing and analysis of over **10.4 million flight records** from 2023–2024 to identify operational bottlenecks and provide data-driven travel recommendations.

### Tech Stack
* **Cloud Infrastructure:** AWS (S3, Glue, Athena) 
* **Querying & Analysis:** SQL, Python 
* **Visualization:** AWS QuickSight 
* **Statistical Methods:** Hypothesis Testing (T-Test), Pearson Correlation

---

### The Solution: Cloud ETL Pipeline
To handle a dataset of this scale, I implemented a serverless architecture on AWS:
* **Data Ingestion:** Stored raw datasets in **AWS S3**.
* **Automated Cataloging:** Used **AWS Glue Crawlers** to scan and define a relational schema for the data.
* **Serverless Analytics:** Performed high-speed aggregations and joins using **AWS Athena**.

### Key Analytical Insight: The "Older Planes" Myth
I tested the hypothesis that older aircraft cause more delays. By sampling aircraft ages from the FAA registry and performing a **Two-Sample T-Test**, I found a **p-value of 0.41**. This confirmed that there is no statistically significant link between aircraft age and flight delays, suggesting that operational factors like weather are more critical.

### Actionable Findings
* **Optimal Travel Window:** Departing between **5 AM and 7 AM** minimizes average delays.
* **Best Day to Fly:** **Tuesday** is statistically the most reliable day for travel.
* **Weather Hotspots:** Hagerstown Regional Airport was identified with the highest percentage of weather-related delays (**5.53%**).

---

### Conclusion
By architecting a cloud-based data solution, I transformed 10 million rows of raw logs into a structured analytical framework, successfully debunking industry myths and identifying optimal travel patterns.

> [Download the Full Technical Report](/uploads/aws_business_report.pdf)