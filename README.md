# Consumer-Behaviour-analytics-dashboard-tableau
Tata Data Visualisation: Empowering Business with Effective Insights Job Simulation on Forage  * Completed a simulation involving creating data visualizations for Tata Consultancy Services  * Prepared questions for a meeting with client senior leadership  * Created visuals for data analysis to help executives with effective decision
# Tata Retail Sales & Customer Behavior Analysis — Excel & Tableau

End-to-end sales, demand, and customer behavior analysis built as part of the **Tata Data Visualisation Job Simulation**.  
This project answers executive-level business questions using Tableau dashboards and extends the analysis through deeper exploration, including RFM-based customer segmentation and multi-metric demand ranking.

---

## Project Overview

This project was completed to simulate how a data analyst supports executive stakeholders such as the **CEO and CMO**.  

The objectives were:

- Analyze revenue trends and seasonality
- Identify top-performing countries and customers
- Evaluate geographic demand for expansion decisions
- Segment customers using behavioral analysis (RFM)
- Deliver insights through clean, executive-ready visual dashboards

The project contains:
- Required stakeholder question analysis (as per simulation instructions)
- Independent extended exploration using advanced segmentation and ranking logic
- Data cleaning aligned strictly with the instructions provided

 
![Consumer Analytics Dashboard](assets/consumer%20analytics%20dashboard.png)
---

# Business Questions & Dashboard Insights

---

## Question 1 — Monthly Revenue Trends for 2011 (CEO)

### Business Objective
The CEO wanted to:
- View revenue trends for 2011 only
- Analyze monthly seasonality
- Understand underlying drivers behind peaks and dips
- Use insights to support forecasting for the next year

### Analytical Approach
- Filtered dataset to 2011
- Aggregated revenue by month
- Extended view by segmenting revenue across RFM customer categories
- Compared performance of Champions, Loyal Customers, Big Spenders, At Risk, and Lost/Low-Value customers

### Key Observations

- Revenue shows visible seasonal variation across months.
- The highest revenue peak reached approximately **53,83,000** (Champions segment).
- Loyal Customers contributed approximately **8,58,000** during peak months.
- Revenue concentration is strongly driven by high-value segments rather than evenly distributed across customer base.
- Late-year months show increased revenue contribution, suggesting seasonal buying behavior.

### Business Interpretation

Revenue growth is not purely time-driven; it is segment-driven.

Champion customers account for a disproportionate share of total sales. Therefore:

- Retention of Champions is critical.
- Loyalty strengthening programs should focus on moving Loyal Customers into Champion status.
- Seasonal campaigns should align with peak buying behavior identified in Q4.

---

## Question 2 — Top 10 Countries by Revenue (Excluding United Kingdom)

### Business Objective
The CMO requested:
- Top 10 countries generating highest revenue
- Exclude United Kingdom
- View quantity sold alongside revenue
- Identify revenue concentration

### Analytical Approach

- Filtered out UK
- Ranked countries by total revenue
- Built cumulative revenue line (Pareto view)
- Calculated running percentage of revenue

### Key Observations

- Revenue concentration is significant.
- By the time Australia is included, cumulative revenue reaches approximately **82%**.
- Only **five countries contribute 82% of total revenue**.
- Remaining countries contribute relatively small portions.

### Business Interpretation

The business is geographically concentrated.

Implications:

- Marketing spend should prioritize top 5 revenue countries.
- Expansion strategy should focus on high-performing non-UK markets.
- Diversification efforts may reduce revenue dependency risk.

---

## Question 3 — Top 10 Customers by Revenue

### Business Objective
The CMO wanted:
- Top 10 customers ranked by revenue
- Visual ordered from highest to lowest
- Identify high-value customer targets for retention

### Analytical Approach

- Aggregated revenue by Customer ID
- Sorted descending
- Selected top 10

### Key Observations

- Revenue distribution among customers is highly skewed.
- A small number of customers generate a large share of revenue.
- Clear descending pattern shows diminishing revenue contribution beyond top tier.

### Business Interpretation

Revenue is customer-concentrated.

Implications:

- High-value customers must receive retention incentives.
- Dedicated account management for top spenders can protect revenue stability.
- Churn risk among top customers could significantly impact overall sales.

---

## Question 4 — Demand Analysis & Expansion Opportunities (CEO)

### Business Objective

The CEO requested:

- Identify regions with strongest product demand
- Exclude UK
- Present all countries in one consolidated view
- Support expansion strategy decisions

### Analytical Approach

Demand was measured using three indicators:

1. Percentage of total revenue
2. Percentage of total quantity sold
3. Percentage of total orders

Each country was evaluated across these three metrics.

### Multi-Metric Demand Ranking

Observations:

- Revenue ranking differs from Order ranking.
- Quantity contribution does not always align with revenue leadership.
- Netherlands ranks highest by revenue.
- Germany ranks highest by order volume in some comparisons.
- The interpretation of demand depends on the business objective.

To create a balanced evaluation:

- A composite Demand Score was calculated by combining all three metrics.
- Each metric contributes equally.
- This provides a ranking that avoids bias toward revenue-only interpretation.

### Final Ranked Top 5 Countries by Composite Demand Score

1. Netherlands
2. Germany
3. EIRE
4. France
5. Australia

### Business Interpretation

Demand should not be defined by revenue alone.

- Revenue reflects monetary strength.
- Quantity reflects volume demand.
- Orders reflect customer activity.

A composite score provides a more strategic expansion indicator.

---

# RFM Customer Segmentation (Extended Analysis)

Beyond required stakeholder questions, customer behavior analysis was conducted using RFM methodology.

---

## RFM Methodology

RFM stands for:

- **Recency** – How recently a customer purchased
- **Frequency** – How often they purchase
- **Monetary** – How much revenue they generate

### Calculation Process

- Max Invoice Date per customer extracted.
- Reference date assumed as 2012 (dataset ends in 2011).
- Days difference calculated for Recency.
- Distinct invoice count used for Frequency.
- Total revenue used for Monetary.
- Each metric converted into 5 percentile-based scores (1–5).
- Scores combined into customer segments.

---

## Customer Segments Created

- Champions
- Loyal Customers
- Big Spenders
- At Risk
- Lost / Low-Value

### Observations

- Champions drive majority of revenue peaks.
- Loyal Customers provide stable recurring revenue.
- Big Spenders generate high monetary contribution but may not purchase frequently.
- At Risk customers show declining recency.
- Lost customers contribute minimal revenue.

### Business Value

- Enables targeted marketing strategy.
- Improves retention decision-making.
- Simplifies customer base understanding.
- Supports churn prediction logic.

---

# Data Cleaning (As Per Simulation Instructions)

Only cleaning steps instructed in the job simulation were performed:

- Removed 10,624 rows with negative quantities.
- Removed 1,179 rows where unit price was zero.

Other identified issues (e.g., missing descriptions, stock code irregularities, minor negative prices) were intentionally left unchanged to strictly follow instructions.

---

# Tools Used

- Microsoft Excel (Cleaning, Pivot Analysis, RFM Calculation)
- Tableau (Dashboard & Visualization)
- Percentile Ranking for segmentation logic

---

# Key Strategic Insights

- Revenue is concentrated in a few customer segments and countries.
- Demand interpretation varies depending on metric (revenue vs orders vs quantity).
- Multi-metric evaluation provides stronger decision support.
- Seasonal peaks align with high-value customer segments.
- Geographic revenue concentration suggests opportunity and risk.

---

# Conclusion

This project demonstrates how executive-level business questions can be translated into structured data analysis, combining:

- Time-series analysis
- Geographic revenue concentration
- Customer revenue ranking
- Multi-metric demand modeling
- Behavioral customer segmentation (RFM)

The result is a complete analytical workflow from raw transactional data to executive-ready strategic insights.
