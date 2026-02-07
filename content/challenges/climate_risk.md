---
title: "Climate Risk & ESG Automation: 1st Place Win"
date: 2025-03-01
layout: "background"
showTableOfContents: true
featured: true
series: ["Hult Business Challenges"]
---

![Bologna Map](/img/eoliann_bologna.png)

### Executive Summary
We worked for **Team EOLIANN**, tasked with optimizing climate risk modeling for infrastructure resilience. We identified a critical bottleneck: the manual collection of wildfire and flood data from the Copernicus Emergency Management Service was taking the client nearly three days per audit.

![Group Picture winning](/img/eoliann_team.jpeg)

### The Challenge: From Data Chaos to Climate Clarity
The goal was to prioritize product features that increase infrastructure climate resilience by identifying high-exposure assets. However, existing datasets from EMDAT and HANZE fell short on asset vulnerability specifics.

![Map Picture](/img/eoliann_transport.jpeg)

### My Technical Solution: The Scraping Engine
I reverse-engineered the HTML structure of the Copernicus portal to identify hidden API endpoints used for different disaster categories. 
* **The Architecture**: Developed a custom Python ingestion engine to automate the fetching of vector ZIP files (SHP and TIF).
* **Geospatial Processing**: Used **GeoPandas** and **Rasterio** to project disaster footprints onto infrastructure maps with high precision.
* **Automation**: Built a "one-click" workflow that reduced a 3-day manual process to a 50-minute automated run.

![Working](/img/eoliann_work.jpeg)

### Business Impact
* **Latency Reduction**: Slashed data collection time by over **90%**.
* **Market Targeting**: Provided the strategic recommendation to target Floods and Wildfires as the highest-growth risk advisory markets.
* **1st Place Award**: Recognized for technical innovation and business scalability.

[View our Python Notebook](/uploads/eoliann_python_notebook.ipynb)

**Technical Toolkit**: Python, GeoPandas, Rasterio, Beautiful Soup, Matplotlib.