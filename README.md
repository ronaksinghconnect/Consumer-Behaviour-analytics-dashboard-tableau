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
| Total Sales | Total Sales RFM |
|-------------|-----------------|
| ![](assets/Total%20sales.png) | ![](assets/Total%20sales%20rfm.png) |
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

![Countries Revenue](assets/countries%20revenue.png)
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

![Top Customers](assets/top%20customers.png)
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
| Rank Top 5 | Top 5 Countries Demand |
|------------|------------------------|
| ![](assets/rank%20top%205.png) | ![](assets/top%205%20countries%20demand.png) |
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
.
..
...
# Tata Retail Sales & RFM Customer Behavior Analysis  
### Executive-Focused Tableau Dashboard Project

This project presents a structured, executive-ready analysis of retail sales and customer behavior using Tableau.  

The analysis is divided into **three strategic dashboards**, each answering a different layer of business decision-making:

1. RFM Analytics Dashboard (Customer Value & Behavior)
2. Comparative Performance Dashboard (Revenue vs Orders vs Demand)
3. Countries & Behavioral Insights Dashboard (Geographic + Churn Intelligence)

Key Analytical Techniques Applied
---
RFM Customer Segmentation Analysis

Multi-Metric Demand Analysis (Revenue + Quantity + Orders)

Time-Series Revenue Trend Analysis

Pareto / Revenue Concentration Analysis

Geographic Revenue & Market Performance Analysis

# 1️⃣ RFM Analytics Dashboard  
### Understanding Customer Value & Revenue Drivers

---
![RFM Analytics Dashboard](assets/RFM%20analytics%20dashboard.png)
## Business Objective

To answer:

- Who are our most valuable customers?
- Which segments drive revenue growth?
- Which customers are at risk of churn?
- How do Recency, Frequency, and Monetary values differ across segments?

---

## Sheet 1 — Total Sales (RFM Segmented Trend)

### What It Shows
Monthly revenue trend segmented by:
- Champions  
- Loyal Customers  
- Big Spenders  
- At Risk  
- Lost / Low-Value  

### Key Metrics Observed

- Peak monthly revenue reached approximately **₹53,00,000+**
- Champions segment drives majority of total revenue spikes.
- Loyal Customers show stable mid-level contribution.
- Big Spenders contribute less frequently but spike occasionally.
- Revenue drops noticeably in final visible month after peak.

### Business Insight

Revenue growth is **segment-driven**, not evenly distributed.

Champions are responsible for revenue volatility and upside peaks.
If Champion retention declines, revenue immediately contracts.

Strategic Action:
- Protect Champions.
- Upgrade Loyal Customers into Champion tier.
- Monitor At-Risk segment before decline accelerates.

---

## Sheet 2 — Customer Category Count

### What It Shows
Distinct count of customers per RFM segment.

### Observed Distribution

- Loyal Customers: **1,440**
- Lost / Low-Value: **958**
- Champions: **910**
- At Risk: **769**
- Big Spenders: **262**

### Business Interpretation

Largest group = Loyal Customers (volume strength).  
Smallest group = Big Spenders (high-value niche).

However:
Revenue contribution is not proportional to count.

This confirms:
High-value revenue comes from smaller segments.

---

## Sheet 3 — Recency Average (Days Since Last Purchase)

### Observed Values

- Lost / Low-Value: **245 days**
- At Risk: **177 days**
- Loyal Customers: **57 days**
- Big Spenders: **55 days**
- Champions: **35 days**

### Insight

Champions purchase most recently.
Lost customers show extreme inactivity.

Recency strongly correlates with revenue strength.

---

## Sheet 4 — Frequency Average (Distinct Orders)

### Observed Values

- Champions: **12 orders**
- Loyal Customers: **3 orders**
- At Risk: **3 orders**
- Big Spenders: **2 orders**
- Lost: **1 order**

### Insight

Champions are behaviorally dominant.

Frequency is the strongest differentiator between Champions and other segments.

---

## Sheet 5 — Monetary Average (Revenue Contribution)

### Observed Values

- Champions: **₹6,253**
- Big Spenders: **₹2,369**
- At Risk: **₹1,448**
- Loyal Customers: **₹875**
- Lost: **₹239**

### Strategic Interpretation

Monetary concentration is extreme.

Champions generate ~7x more revenue than Loyal Customers on average.

Revenue risk is heavily tied to this segment.

---

# 2️⃣ Comparative Dashboard  
### Relationship Between Revenue, Orders & Demand

---
![Comparative Dashboard](assets/comparitive%20dashboard.png)
## Sheet 1 — Revenue vs Number of Orders

### What It Shows
Scatter plot comparing:
- Sum of Revenue
- Distinct Invoice Count

### Observations

- Champions cluster in high revenue + high order zone.
- Some customers show high revenue but low order frequency.
- Median lines highlight separation between majority and high performers.
- Revenue ranges from very low to over **₹1,00,000+** per customer.

### Insight

Not all high-revenue customers are high-frequency.

Some customers are bulk buyers.

This distinction is critical for retention strategy.

---

## Sheet 2 — Quantity vs Revenue (RFM Customers)

### Observations

- Strong positive relationship between revenue and quantity.
- Some outliers generate extremely high revenue (~**₹2,50,000+**).
- Champions dominate upper-right quadrant.
- Lost and At-Risk cluster in low revenue, low quantity zone.

### Interpretation

Revenue growth is primarily volume-driven.

High-quantity buyers are key revenue multipliers.

---

## Sheet 3 — Top 10 Revenue Products + RFM Segmentation

### Observations

- Revenue per product ranges approx **₹27,00,000 to ₹45,00,000**.
- Champions dominate contribution across all top SKUs.
- Loyal and Big Spenders contribute secondary layers.
- Certain stock codes consistently outperform others.

### Insight

Product demand is highly segment-driven.

Champions influence product success.

SKU-level marketing can be tied to high-value segments.

---

## Sheet 4 — Customer Base Distribution (%)

### Observed Breakdown

- Loyal Customers: **33.19%**
- Lost / Low-Value: **22.08%**
- Champions: **20.97%**
- At Risk: **17.72%**
- Big Spenders: **6.04%**

### Strategic View

Champions are only ~21% of customers  
But generate disproportionate revenue.

This is a classic Pareto structure.

---

# 3️⃣ Countries & Behavior Dashboard  
### Geographic Revenue & Risk Analysis

---
![Countries and Behaviour Dashboard](assets/countries%20and%20behaviour%20dashboard.png)
## Sheet 1 — Top 5 Countries by Revenue

### Observations

- United Kingdom: **₹73.2L+**
- Netherlands: ~₹2.85L
- EIRE: ~₹2.65L
- Germany: ~₹2.28L
- France: ~₹2.09L

### Insight

UK dominates revenue massively.

Revenue concentration risk is high.

Diversification required.

---

## Sheet 2 — Bottom 5 Countries

### Observations

- Brazil: ~₹1,143
- RSA: ~₹1,002
- Czech Republic: ~₹826
- Bahrain: ~₹548
- Saudi Arabia: ~₹145

### Interpretation

These markets are underdeveloped.

Expansion viability should consider:
- Demand consistency
- Marketing cost efficiency

---

## Sheet 3 — Churn % (60 Days)

### Observed Values

- Lost / Low-Value: **100%**
- At Risk: **100%**
- Big Spenders: **12%**
- Loyal Customers: **12%**
- Champions: **0%**

### Critical Insight

Champions show zero churn in 60-day window.

At Risk and Lost segments are fully disengaged.

Churn prevention should focus before customers transition into Lost.

---

## Sheet 4 — Median Days to 2nd Purchase

### Observed Values

- Champions: **33 days**
- At Risk: **55 days**
- Loyal Customers: **70 days**
- Lost: **71 days**
- Big Spenders: **83 days**
Median was used because second-purchase timing is skewed by extreme delays, and median shows the typical customer behavior without outlier distortion
### Insight

Champions repurchase fastest.

Longer repurchase gaps correlate with lower engagement.

Second purchase timing is a predictive retention indicator.

---

# Strategic Business Conclusions

1. Revenue is highly concentrated in Champion customers.
2. Geographic revenue is heavily dependent on UK.
3. Quantity and revenue are positively correlated.
4. Customer behavior segmentation provides actionable retention paths.
5. Early churn signals are visible in Recency and 2nd purchase timing.
6. Product-level performance is segment-driven.
7. Revenue sustainability depends on protecting top-tier customers.

---

# Tools Used

- Microsoft Excel (Data Cleaning & RFM Calculation)
- Tableau (Dashboard & Visualization)
- Percentile-Based Segmentation Logic

---

# Executive Summary

This project demonstrates how structured RFM segmentation combined with:

- Time-series revenue analysis
- Geographic concentration analysis
- Order vs revenue relationship modeling
- Demand ranking logic
- Churn behavior monitoring

can transform raw transaction data into strategic, decision-support intelligence.

The dashboards are designed for leadership-level clarity, focusing on risk exposure, growth levers, and customer value concentration.
