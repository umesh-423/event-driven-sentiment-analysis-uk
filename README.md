# Event-Driven Public Sentiment Analysis (UK Cost of Living)

This project analyses how public sentiment shifted **before vs after** the UK **Energy Price Guarantee announcement (8 September 2022)** using social media data.  
It combines a **Python-based sentiment analysis pipeline** with an **interactive Power BI dashboard** to identify sentiment trends and uncover the key drivers behind negative public reactions.

---

## 📊 Dashboard Overview

### Page 1 — Executive Summary
- High-level KPIs comparing **Before vs After** the announcement
- Overall sentiment shift and change in negative sentiment share

### Page 2 — Event Impact Timeline
- Daily sentiment trend over time
- Event-day marker highlighting the policy announcement
- Posting volume to contextualise sentiment changes

### Page 3 — Drivers of Negative Sentiment
- Top keywords driving negative sentiment
- Real high-confidence negative tweet examples
- Insights translated into actionable implications

---

## ❓ Business Question

**How did public sentiment change following the Energy Price Guarantee announcement, and what themes drove negative public reactions?**

---

## 📌 Key Findings

- **Average sentiment declined** from **-0.23 (Before)** to **-0.29 (After)** the announcement.
- **Negative sentiment increased** from **66.79%** to **70.44%**, indicating heightened public concern.
- Timeline analysis shows a **sharp drop in sentiment immediately after 8 Sept 2022**.
- Keyword analysis reveals that negative sentiment was primarily driven by:
  - Cost
  - Cost of living
  - Crisis-related language
- Example tweets confirm that concerns were grounded in **real household and financial pressures**, rather than isolated reactions.

---

## 🧠 Approach

### 1️⃣ Data Preparation
- Parsed and standardised tweet timestamps
- Cleaned tweet text (URLs, mentions, punctuation)
- Created an **event window** (Before vs After the announcement)

### 2️⃣ Sentiment Analysis (Python)
- Applied **VADER sentiment analysis** to compute sentiment scores
- Used absolute sentiment score as a **confidence proxy**
- Filtered out low-confidence sentiment to improve signal quality

### 3️⃣ Feature Engineering & KPIs
Generated structured outputs for BI analysis:
- `daily_kpi.csv` — daily sentiment and posting volume
- `period_summary.csv` — Before vs After comparison
- `negative_drivers.csv` — top negative sentiment keywords
- `tweets_scored.csv` — tweet-level data for validation

### 4️⃣ Power BI Visualisation
- Executive KPI cards
- Event-driven sentiment timeline with marker
- Negative driver analysis with real tweet examples
- Insight-focused dashboard design for non-technical stakeholders

---

## 🛠 Tech Stack

- **Python:** pandas, regex, vaderSentiment  
- **Data Analysis:** Jupyter / Google Colab  
- **Business Intelligence:** Power BI  
- **Version Control:** GitHub  

---

## 📂 Repository Structure



---

## ▶️ How to Reproduce

1. Run the notebook in `notebooks/sentiment_pipeline.ipynb`
2. Generated CSVs will be saved in `data/processed/`
3. Open the Power BI file and refresh data sources
4. Explore the dashboard pages for insights

---

## 👩‍💻 Author

**Umesh Iyer**  
📍 London, UK  
🔗 LinkedIn: https://www.linkedin.com/in/umesh-iyer04/  
💻 GitHub: https://github.com/umesh-423

---

## 📌 Why This Project Matters

This project demonstrates:
- Event-driven analytical thinking
- End-to-end data analysis workflow
- Strong storytelling with data
- Ability to translate raw social media data into actionable insights

It is designed to reflect **real-world analyst work**, not just visualisation.



