# Viraj Pahade — Data Analytics Portfolio

**MSc Business Analytics (Distinction) — Queen Mary University of London**
Business Analyst | Data Analyst | SQL · Python · Power BI · NLP
📍 London, UK | 🔗 [LinkedIn](https://linkedin.com/in/virajpahade) | ✉️ virajpahade1008@gmail.com
**Right to work in the UK — UK Graduate Visa until early 2028; sponsorship needed after that**

---

## At a glance

| Project | Business question | Headline result |
|---|---|---|
| [Airline stocks vs oil & sentiment](#1-bloomberg-terminal--oil-price-sentiment--airline-stock-analysis) | How exposed are airline stocks to fuel prices and investor mood? | A 1% rise in Brent → **−0.18%** airline returns |
| [Hotel review sentiment NLP](#2-hotel-review-sentiment-nlp-classifier--500000-records) | What drives negative value perception, and does booking channel matter? | **88%** accuracy; OTA guests rate value worse than direct guests |
| [Customer segmentation](#3-customer-segmentation--personalisation-analysis) | Which customer groups exist, and how should each be treated? | **3 cohorts**, each with its own retention strategy |

> **About the data:** The original analysis used licensed Bloomberg Terminal data and proprietary MSc project data, and neither can be published. The notebooks here show the method on **synthetic demo data**, so their outputs will **not** match the results quoted below, which come from the original work. Each project is being rebuilt on a real public dataset: 515K Hotel Reviews (Kaggle), UCI Online Retail II, and Yahoo Finance/FRED for oil and airline prices.

---

## Projects

### 1. Bloomberg Terminal — Oil Price, Sentiment & Airline Stock Analysis
**Tools:** Python · SQL · Bloomberg Terminal · Regression Modelling · Event Study Methodology
**Dataset:** ~1,750 daily observations across 8 global airlines (IAG, Lufthansa, Air France-KLM, Delta, United, American, Singapore Airlines, Cathay Pacific)

**What I did:**
- Extracted and validated financial market data (equity returns, Brent crude prices, investor sentiment) using the Bloomberg Terminal
- Estimated each airline's oil price beta with OLS regression and measured how prices reacted to sentiment shocks with an event study
- Turned the results into recommendations for risk and investment teams

**Key findings:**
- A **1% rise in Brent crude reduces airline stock returns by approximately 0.18%**
- **Negative investor sentiment drives stock declines of up to 0.7% within two trading days**
- American Airlines was the most exposed to oil prices and Singapore Airlines the least, consistent with differences in their fuel-hedging programmes

📂 [View project notebook](./bloomberg_airline_analysis.ipynb)

---

### 2. Hotel Review Sentiment NLP Classifier — 500,000+ Records
**Tools:** Python · Scikit-learn · NLTK · SpaCy · TF-IDF · Text Classification
**Dataset:** 500,000+ hotel reviews

**What I did:**
- Built an end-to-end NLP pipeline that takes raw review text through to a trained classifier
- Prepared the text with tokenisation, stopword removal and lemmatisation (SpaCy), then built TF-IDF features from unigrams and bigrams
- Compared Naive Bayes, Logistic Regression and Linear SVM; the final model (Linear SVM) reached **88% accuracy**

**Key business insight:**
- **Guests who booked through OTAs (Booking.com, Expedia) rated value systematically worse than direct-booking guests paying the same room rate**
- The root cause was the expectations set at the booking stage, not the price. Revenue and channel strategy teams can act on this directly.

📂 [View project notebook](./hotel_nlp_sentiment.ipynb)

---

### 3. Customer Segmentation & Personalisation Analysis
**Tools:** Python · Scikit-learn (K-Means, PCA) · Pandas · Matplotlib · Seaborn

**What I did:**
- Segmented customers on RFM-style features: recency, frequency, monetary value, tenure and session time
- Chose k = 3 for business usability: three segments map to three distinct actions, after comparing elbow and silhouette results for k = 2–9
- Profiled each segment and recommended a strategy for each

| Segment | Share | Strategy |
|---|---|---|
| High-Value Loyalists | 30% | Loyalty rewards, premium upsell |
| Mid-Tier Actives | 40% | Re-engagement and frequency incentives |
| At-Risk Churners | 30% | Win-back offers, churn prediction |

📂 [View project notebook](./customer_segmentation.ipynb)

---

## Run the notebooks

```bash
git clone https://github.com/viraj1308/data-analytics-portfolio.git
cd data-analytics-portfolio
pip install pandas numpy matplotlib seaborn scipy scikit-learn jupyter
jupyter notebook
```

Each notebook generates its own synthetic data, so no downloads are needed.

---

## Technical Skills

| Category | Tools |
|---|---|
| Languages | Python (Pandas, Scikit-learn, NLTK, SpaCy), SQL |
| BI & Visualisation | Power BI (DAX, Power Query), Advanced Excel |
| Databases | PostgreSQL, MySQL, SQLite, BigQuery |
| Methods | Regression Modelling, Event Study, NLP, Clustering, EDA |
| Delivery | Agile, Jira, Confluence, BRD/FRD Authoring, UAT |
| Other | Bloomberg Terminal, Generative AI / LLMs |

---

## Certifications

- McKinsey Forward Programme — McKinsey & Company
- Microsoft Power BI PL-300 — in progress
- Associate Data Analyst — DataCamp
- SQL & Predictive Analytics — DataCamp
- Python for Data Analysis — DataCamp
- Generative AI — Udemy
- Business Analysis Foundations — LinkedIn Learning

---

*Open to Business Analyst, Data Analyst and BI Analyst roles across the UK.*
