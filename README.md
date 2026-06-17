# 👥 Customer Behavior & Segmentation Analysis

Nigeria E-Commerce Operations | 2023

Analyst: Ibibo Ataisi Justin — Business & Data Analyst  
Tools: Microsoft Excel · SQL · Power BI  
Scope: 300 customer records · 12 months · 5 product categories · Multiple Nigerian cities

---

## 📌 Project Background

A Nigerian e-commerce business serving customers across multiple cities had accumulated a full year of customer transaction records but had no systematic way of understanding who its customers were, how they behaved, or which segments were most valuable. The business was treating all customers the same — sending identical communications, offering the same promotions, and investing equal effort regardless of customer value.

This project applies RFM (Recency, Frequency, Monetary) Segmentation to identify distinct customer groups so the business can tailor its engagement strategy — investing more in high-value customers, re-engaging at-risk ones, and understanding the behavioral patterns that drive purchasing decisions.

---

## ❓ Business Questions Answered

- Who are the highest-value customers and what do they buy?
- Which customers are at risk of churning and need re-engagement?
- What are the purchasing patterns across age groups and gender?
- Which product categories drive the most repeat purchases?
- Which payment methods are most associated with high-value transactions?
- Which cities generate the most active and valuable customer bases?

---

## 🗂️ Dataset Overview

| Attribute | Detail |
|---|---|
| Records | 300 customer transactions |
| Time Period | January – December 2023 |
| Cities | Lagos, Abuja, Port Harcourt, Kano, Ibadan, Enugu, Kaduna |
| Product Categories | Electronics, Fashion, Groceries, Home & Living, Beauty |
| Payment Methods | Bank Transfer, Card, Cash |
| Key Fields | Customer ID, Age, Gender, City, Purchase Date, Category, Order Value, Purchase Frequency, Last Purchase Date, Payment Method |

---

## 🧹 Data Quality Issues & Resolutions

| Issue Identified | Impact if Unresolved | Resolution Applied |
|---|---|---|
| Duplicate Customer IDs | Same customer counted multiple times | Removed duplicates, kept most recent record |
| Age outliers (e.g. 999, 150) and blanks | Age-group analysis distorted | Removed outliers, filled blanks with city average |
| Negative Order Values | Revenue calculations understated | Removed as invalid transactions |
| Inconsistent Gender (M, Male, MALE, m) | Gender segment split into 8+ false categories | Standardized to Male / Female only |
| Mixed date formats across 2 columns | Recency and frequency calculations incorrect | Standardized all dates to DD/MM/YYYY |
| City names with trailing spaces | City analysis split across duplicate entries | Cleaned using TRIM() |
| Inconsistent category names | Category revenue undercounted | Standardized to Title Case using PROPER() |
| Mixed payment method formats | Payment analysis fragmented | Standardized to 3 values: Bank Transfer, Card, Cash |
| Blank cells in key columns | Segment assignment impossible | Filled using logical reference lookups |

---

## 🔬 Segmentation Framework — RFM Analysis

RFM is a proven, data-driven framework for understanding customer value across three dimensions:

| Dimension | Definition | Why It Matters |
|---|---|---|
| R — Recency | How recently did the customer purchase? | Recent buyers are more likely to respond to offers |
| F — Frequency | How many times did they purchase? | Frequent buyers demonstrate loyalty |
| M — Monetary | How much have they spent in total? | High spenders represent the most valuable segment |

### Customer Segments

| Segment | Definition | Business Priority |
|---|---|---|
| 🏆 Champions | Bought recently, buy often, spend the most | Reward and retain — your best customers |
| 💛 Loyal Customers | Buy regularly with moderate to high spend | Upsell and cross-sell to increase order value |
| ⚠️ At-Risk Customers | Were active but haven't purchased recently | Re-engagement campaigns — win them back |
| ❌ Lost / Inactive | Long time since purchase, low frequency | Low-cost reactivation or remove from active marketing |

---

## 📈 Analysis Performed

| Analysis | Method |
|---|---|
| RFM Scoring & Segment Assignment | Excel calculated columns — Recency days, Frequency count, Monetary sum per customer |
| Segment Distribution | Count of customers per RFM segment |
| Revenue Contribution by Segment | SUMIF of Order Value per segment |
| Purchase Pattern by Age Group | Age brackets (18–25, 26–35, 36–50, 51+) vs frequency and spend |
| Category Preference by Segment | Cross-tabulation of segment vs product category |
| City-Level Customer Activity | Customer count and total spend by city |
| Payment Method Analysis | Order value distribution by payment method |
| Recency Distribution | Days-since-last-purchase histogram to identify churn risk |

---

## 📊 Dashboard Features

The Power BI dashboard includes:

- KPI Cards — Total Customers, Total Revenue, Average Order Value, Average Purchase Frequency
- Donut Chart — Customer distribution by RFM Segment
- Bar Chart — Revenue contribution by Segment
- Bar Chart — Purchase frequency and spend by Age Group
- Bar Chart — Top categories by Segment
- Map Visual — Customer distribution by City
- Table — Top 20 Champion customers by Monetary value
- Slicers — Segment, Category, City, Gender, Payment Method

---

## 💡 Key Insights

- Identified the top customer segment by revenue contribution
- Quantified the percentage of customers at risk of churning and their estimated revenue value
- Revealed which age group is most associated with high-frequency, high-value purchasing
- Uncovered product categories with the highest repeat purchase rates
- Highlighted cities with the most commercially active customer bases
- Identified payment method preferences among high-value customers

---

## 🧠 Skills Demonstrated

| Skill | Application |
|---|---|
| Data Cleaning & Validation | Resolved 9 categories of data quality issues across 300 records |
| Excel Formulas | SUMIF, TRIM, PROPER, DATEDIF, IF, VLOOKUP, COUNTIF |
| RFM Segmentation | Scoring and classifying 300 customers across 3 dimensions |
| Pivot Tables | Cross-tabulation of segments, categories, cities, and age groups |
| Power BI Dashboard Development | Multi-visual interactive dashboard with cross-filtering slicers |
| Customer Analytics | Translating RFM scores into actionable engagement strategies |
| Business Analysis | Connecting segment findings to specific commercial recommendations |
| Data Storytelling | Communicating customer insight clearly to non-technical stakeholders |

---

## 📁 Repository Contents

- Customer_Segmentation_MESSY.xlsx — Original raw dataset
- Customer_Segmentation_CLEANED.xlsx — Cleaned and RFM-scored dataset
- Customer_Segmentation_Dashboard.pbix — Power BI dashboard file
- Project_Overview.docx — Full project documentation
- Dashboard_Screenshot.png — Preview of final dashboard

---

## 🤝 Let's Connect

Ibibo Ataisi Justin  
Business & Data Analyst | Power BI · SQL · Excel

📍 Port Harcourt, Nigeria ·
