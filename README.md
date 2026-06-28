# Regional Sales Analysis 

Analyzing 5 years of regional sales data to uncover revenue drivers, seasonal trends, top products, channel profitability, and budget performance — enabling smarter pricing, promotions, and market expansion decisions.

---

# Brief Summary

An end-to-end sales analysis project on XYZ Co.'s 2014–2018 regional sales dataset — involving multi-sheet Excel merging, data cleaning, feature engineering, EDA using Python, and an interactive Power BI dashboard — to answer: "How can XYZ Co. leverage 5 years of historical sales data to pinpoint growth levers and optimize strategy?"

---

# Overview

This project analyses and visualizes regional sales data across products, channels, and U.S. regions to uncover trends, evaluate profitability, and support strategic decision-making. It covers multi-table data merging, feature engineering (profit, margin %), seasonal trend analysis, top SKU identification, channel profitability comparison, regional performance, and 2017 budget vs. actual tracking — all powered by Python and visualized in Power BI.

---

# Problem Statement

Sales teams often lack a clear, data-driven understanding of regional performance, making it difficult to identify growth opportunities and optimize resources. This project aims to analyse and visualize regional sales data to uncover trends, evaluate profitability, and support strategic decision-making.

What's the Business Question?


Inconsistent revenue and profit performance across U.S. regions
Lack of visibility into seasonal swings, top SKUs, and channel profitability
Goal: Leverage 5 years of historical data to pinpoint growth levers and optimize strategy

---

# Dataset

| Sheet | Description |
|-------|-------------|
| Sales Orders | Core transactions — orders, quantities, prices, revenue |
| Customers | Customer names and IDs |
| Products | Product names, descriptions, and unit costs |
| Regions | Delivery region details |
| State Regions | State-to-region mapping |
| 2017 Budgets | Budget targets per product for 2017 |

---

# Tools & Technologies

| Tool | Purpose |
|------|---------|
| Python (Jupyter Notebook) | Data merging, cleaning, feature engineering & EDA |
| Pandas / NumPy | Data manipulation |
| Matplotlib / Seaborn / Squarify | Visualizations |
| Power BI | Interactive dashboard & reporting |

---

# Methods

1. Data Loading — Loaded all 6 sheets from Regional_Sales.xlsx into separate DataFrames.
2. Multi-Sheet Merging — Performed 5 sequential left joins: Sales Orders ← Customers ← Products ← Regions ← State Regions ← 2017 Budgets.
3. Data Cleaning — Dropped redundant duplicate columns, standardized all column names to lowercase with underscores, kept 15 relevant features, renamed columns for clarity (line total → revenue, total unit cost → cost), set budget to NaN for all non-2017 rows, and removed incomplete Jan–Feb 2018 records to avoid skewed trend analysis.
4. Feature Engineering — Created total_cost (quantity × cost), profit (revenue − total_cost), profit_margin% ((profit / revenue) × 100), and extracted month and year from order_date.
5. Exploratory Data Analysis — Monthly revenue trend (2014–2018), seasonal aggregation by month, top 10 products by revenue, unit price distribution for top 10 products, channel revenue share (treemap), channel profit margin comparison, Average Order Value (AOV) distribution, top 10 states by revenue & order count, revenue & order share by region, top 10 customers by revenue, and correlation heatmap.

---

✅ Results & Conclusion

The analysis successfully identified XYZ Co.'s key revenue and profit drivers across 5 years of sales data. Top products, high-margin channels, and dominant regions emerged as critical levers for growth. Regional disparity in performance highlights markets where focused investment could yield strong returns. The 2017 budget vs. actual comparison provides a reliable benchmark for future planning. These insights directly support strategic decisions around pricing, promotions, and market expansion — reducing concentration risk while optimizing profitability.

---

# Author & Contact

|    |      |
|----|------|
|Name | KRISHNA |
|LinkedIn | https://www.linkedin.com/in/krishna-krishna-26a106231/ |
|GitHub | https://github.com/ |


⭐ If you found this project helpful, consider giving it a star!
