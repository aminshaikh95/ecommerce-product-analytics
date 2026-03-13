# E-Commerce Product Analytics — Mixpanel

A product analytics project analyzing user behavior, funnel performance, and retention on a simulated e-commerce platform using Mixpanel.

---

## Project Summary

This project uses a synthetic dataset of 2,853 users across 7 countries and 6 product categories to answer core product analytics questions. All analysis and reporting was done in Mixpanel.

---

## Dashboard Reports

**Today Active Users** — 1,529 unique users active today, up 4,678% compared to the previous day.

**Weekly Active Users** — 1,639 unique users active in the past 7 days, up 498% compared to the previous week.

**Unique Purchases by Product Category** — Tracks monthly purchase trends across 6 categories: Home & Garden, Electronics, Beauty, Books, Sports, and Clothing. Home & Garden and Electronics consistently lead in purchase volume across the 6-month period.

**Active Users by Country** — Poland (58), Germany (54), Spain (50), Netherlands (47), France (38), USA (37), UK (35).

**Retention** — 55.58% of users returned within the first week. Retention drops sharply after week one, stabilizing at a low but consistent level through week 12.

**Purchase Conversion Funnel** — 5-step funnel tracked over 12 months:

| Step | Users | Conversion |
|---|---|---|
| User Signed Up | 2,853 | 100% |
| Product Viewed | 1,522 | 53.35% |
| Added to Cart | 532 | 21.81% |
| Checkout Started | 107 | 32.23% |
| Purchase Completed | 52 | 48.6% |

Overall end-to-end conversion rate: 1.82%

---

## Key Findings

The largest drop-off in the funnel occurs between Product Viewed and Added to Cart, where over 78% of browsing users do not add anything to their cart. This is the highest-leverage point for conversion optimization.

Retention falls sharply after the first week, suggesting that re-engagement campaigns in days 3 to 7 post-signup would have the greatest impact on long-term user retention.

Home & Garden and Electronics are the strongest performing categories by purchase volume and show consistent month-over-month growth.

---

## Tools

- Python (Pandas, NumPy) — synthetic data generation and Mixpanel API ingestion
- Mixpanel — funnel analysis, retention analysis, segmentation, and dashboard
- Google Colab — development environment

---

## How to Run

1. Open `mixpanel_data_generator.ipynb` in Google Colab
2. Add your Mixpanel Project Token and API Secret in the credentials cell
3. Run all cells in order
4. Open Mixpanel and build reports using the imported event data

---

## Author

Amin | Data Analyst | Berlin, Germany

MSc Data Analytics | MBA Digital Marketing | BBA Marketing

[LinkedIn](#) | [GitHub](#)
