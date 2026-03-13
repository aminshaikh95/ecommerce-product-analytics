# E-Commerce Product Analytics — Mixpanel

A product analytics project built to analyze user behavior, funnel performance, and retention patterns on a simulated e-commerce platform. The analysis was conducted in Mixpanel using a synthetic dataset generated in Python.

---

## Overview

This project simulates six months of user activity on an e-commerce platform with 3,000 users across seven countries. The goal was to identify where users drop off in the purchase funnel, which acquisition channels bring the highest-quality users, and how retention varies across cohorts.

The findings are presented as an interactive Mixpanel dashboard covering funnel analysis, weekly retention, geographic distribution, and revenue by channel.

---

## Business Questions

- At which step of the purchase funnel do we lose the most users?
- Which acquisition channel produces the highest conversion rate?
- How well do we retain users after their first visit?
- Which product categories and markets drive the most revenue?

---

## Dataset

The dataset was synthetically generated using Python to simulate realistic e-commerce behavior. It includes 3,000 users and approximately 17,000 events spanning 12 months.

**Users table includes:**
- User ID, acquisition channel, country, device type, age group, preferred category, signup date

**Events tracked:**
- User Signed Up
- Product Viewed
- Added to Cart
- Checkout Started
- Purchase Completed
- Review Submitted

**Acquisition channels:** Organic, Paid Search, Referral, Social Media, Email

**Countries:** Germany, USA, UK, France, Netherlands, Spain, Poland

---

## Tools

- Python (Pandas, NumPy) — data generation and Mixpanel API ingestion
- Mixpanel — funnel analysis, retention analysis, segmentation, and dashboard
- Google Colab — development environment
- GitHub — version control and portfolio hosting

---

## Key Findings

**Funnel Analysis**

The biggest drop-off in the purchase funnel occurs between Product Viewed and Added to Cart, where approximately 77% of users continue but only 23% proceed to add an item to their cart. Overall end-to-end conversion from signup to purchase sits at around 3%.

**Retention**

Week-one retention stands at approximately 55%, which drops sharply by week two. This indicates that re-engagement in the first seven days is critical and represents the highest-leverage opportunity for improving long-term user value.

**Acquisition Channels**

Referral users convert at a significantly higher rate than other channels, suggesting that referred users arrive with a higher level of trust and intent. Social Media drives volume but underperforms on conversion, pointing to a potential budget reallocation opportunity.

**Geographic Distribution**

Poland, Germany, and Spain represent the three largest user segments in this dataset, which would inform localization and marketing priorities in a real-world scenario.

---

## Dashboard

The Mixpanel dashboard includes the following reports:

- Purchase Conversion Funnel — 5-step funnel from signup to purchase
- Weekly Cohort Retention — retention curve across 12 weeks
- Active Users by Country — geographic breakdown of user activity
- Daily and Weekly Active Users — engagement trends over time

Screenshots of the dashboard are included in the `/screenshots` folder of this repository.

---

## Project Structure

```
ecommerce-product-analytics/
│
├── mixpanel_data_generator.ipynb   # Data generation and Mixpanel ingestion
├── screenshots/                    # Mixpanel dashboard and report screenshots
│   ├── funnel_analysis.png
│   ├── retention_chart.png
│   ├── dashboard_overview.png
│   └── country_breakdown.png
├── README.md
└── LICENSE
```

---

## How to Run

1. Open `mixpanel_data_generator.ipynb` in Google Colab
2. Run all cells in order
3. Add your Mixpanel Project Token and API Secret in the credentials cell
4. Run the final cell to send events to Mixpanel
5. Open Mixpanel and build reports using the event data

---

## Author

Amin | Data Analyst | Berlin, Germany

MSc Data Analytics | MBA Digital Marketing | BBA Marketing

[LinkedIn](#) | [GitHub](#)
