---
title: "AparaviBot: Architecting an AI-Driven Medtech Intelligence Platform"
date: 2025-04-08
draft: false
description: "Developing a dual-mode RAG chatbot using Aparavi's Data Toolchain, OpenAI GPT-4, and Weaviate to analyze medical device regulations and developer community insights."
tags: ["AI Engineering", "RAG", "Vector Databases", "Aparavi", "AWS", "Python", "Medtech"]
categories: ["Data Engineering", "Artificial Intelligence"]
showTableOfContents: true
---

### Project Overview
AparaviBot is a high-performance AI solution designed to bridge the gap between unstructured regulatory data and real-time community insights. Built as part of the Aparavi Innovation Challenge, the platform utilizes an automated data toolchain to process complex medical device documentation and social data, providing researchers and developers with a centralized intelligence hub.

### Tech Stack
* **Data Toolchain:** Aparavi Data Intelligence & Toolchain for AI
* **Infrastructure:** AWS S3 (Data Lake)
* **Vector Database:** Weaviate (Semantic Search & Retrieval)
* **LLM & Embeddings:** OpenAI GPT-4 and `text-embedding-3-small`
* **Frontend:** Gradio (Web Interface)
* **Integration:** Python (PRAW for Reddit, GitHub REST API, Stack Exchange API)

---

### The Challenge: Unstructured Data Complexity
The Medtech industry generates vast amounts of unstructured data like FDA approval summaries, McKinsey reports, and regulatory guides that are difficult to index and query efficiently. Traditional RAG pipelines often struggle with "dirty" data and lack of context. The goal was to minimize the "time-to-insight" by automating the cleaning, tagging, and chunking process.

### The Solution: The Aparavi Data Pipeline
I implemented a serverless pipeline that transforms raw documents into high-fidelity semantic vectors:

1.  **Ingestion & Parsing:** Publicly available FDA and MedTech Dive documents were ingested into an **AWS S3** bucket and processed through the **Aparavi Document Parser**.
2.  **Enriched Metadata Tagging:** Unlike standard chunking, Aparavi automatically tagged document segments with metadata such as *Device Name*, *Year of Approval*, and *Medical Category* (e.g., Cardiac, Diagnostic).
3.  **Vectorization:** These enriched chunks were embedded using OpenAI and stored in **Weaviate**, where the added metadata allowed for highly context-aware semantic retrieval.

---

### Feature Deep Dive: Dual-Mode Intelligence

#### 1. Health Chatbot (Regulatory Intelligence)
This mode acts as a specialized assistant for the medical device sector. It allows users to query over 10 million data points, including:
* **FDA Approval Summaries (2022-2024):** Instant retrieval of device classifications and approval dates.
* **Market Research:** Summarized insights from McKinsey and MedTech Dive.
* **Reimbursement Guides:** Navigating complex regulatory landscapes for device commercialization.

#### 2. Miscellaneous Chatbot (API Integration)
To capture real-time technical sentiment, I built connectors to developer hubs:
* **Reddit & Stack Overflow:** Monitoring trends in Data Science and Health Tech.
* **GitHub:** Tracking commits and issues across relevant repositories to gauge development momentum.

---

### Key Engineering Insights
* **Automated Tagging Value:** Using Aparavi’s automatic classification reduced the manual effort required for data preparation by approximately 60%, significantly accelerating the model training phase.
* **Semantic Precision:** The integration of metadata into the vector search ensured that the LLM (GPT-4) provided more accurate, "hallucination-free" responses by grounding the output in specific regulatory context.
* **UX Design:** Implemented a simulated typing stream in Gradio to enhance the user experience and mimic human-like interaction.

---

### Conclusion
AparaviBot demonstrates the power of a modern AI toolchain in solving real-world data problems. By automating the organization of unstructured data, the platform enables Medtech professionals to move from data collection to strategic decision-making in a fraction of the traditional time.

### Watch the Demo Video
{{< youtube Bk8mgByhKbU >}}

