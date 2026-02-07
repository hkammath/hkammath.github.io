---
title: "EXP-EYE-R: 1st Place"
date: 2026-02-07
layout: "background"
showTableOfContents: true
featured: true
series: ["Hult Business Challenges"]
---

### Executive Summary
Food waste in U.S. supermarkets accounts for 16 billion lbs of waste and $2 billion in disposal costs annually. We developed **EXP-EYE-R**, an AI-powered camera solution to spot nearing-expiration products in real-time.

![Group Picture EXPEYER](/img/exp_ey_r_team.jpeg)

### Technical Solution Architecture
I led the prototype design for a camera-based detection system that integrates with store management dashboards.
* **Object Detection**: Implemented **YOLOv8** to identify product types and shelf positions.
* **Date Extraction**: Used **OCR (Pytesseract)** to read expiry dates from product packaging, even in varying shelf lighting.
* **Tracking**: Integrated **DeepSORT** for real-time tracking of products as they are moved by customers or staff.
* **Backend**: Developed a high-availability **Spring Boot** backend with scheduled refreshes to update store databases.

[View our MVP technical documentation](/uploads/mvp_design.pdf)

### Demo & Business Impact
* **Efficiency**: Eliminated manual expiry checks, allowing managers to act fast with discounts or donations.
* **Sustainability**: Directly addressed the 3rd largest source of methane emissions in the U.S. by reducing retail waste.

### Demo Video
{{< youtube 9hO-c1LeIX8 >}}

**Technical Toolkit**: YOLOv8, DeepSORT, Pytesseract, Spring Boot, Python, REST APIs, PowerBI.