# 📊 SQL Business Analytics Project


A SQL-based business analytics project built on top of a structured Data Warehouse. It transforms Gold layer data into actionable insights through a series of analytical modules — covering sales trends, customer segmentation, product performance, and executive-level reporting views.

> 🔗 *This project consumes the Gold layer produced by the [SQL Data Warehouse Project](https://github.com/Mersad-MAZ/sql-data-warehouse-project).*

---

## 📋 Table of Contents

- [Dataset](#dataset)
- [Analysis Modules](#analysis-modules)
- [Business Questions Answered](#business-questions-answered)
- [Reporting Views](#reporting-views)
- [Project Structure](#project-structure)
- [Skills Demonstrated](#skills-demonstrated)
- [About This Project & Author](#about-this-project--author)

---

## 🗄️ Dataset

The analysis is built on the Gold layer from the companion Data Warehouse project, which integrates CRM and ERP source systems into a clean star schema.

| Table | Type | Description |
|-------|------|-------------|
| `gold.dim_customers` | Dimension | Customer master with demographic and behavioral attributes |
| `gold.dim_products` | Dimension | Product catalog with category and pricing information |
| `gold.fact_sales` | Fact | Transactional sales records linked to customers and products |

---

## 🔬 Analysis Modules

Each script addresses a distinct analytical technique applied to the business dataset:

| # | Module | What It Does |
|---|--------|--------------|
| 1 | **Change Over Time** | Tracks sales and revenue trends across months and years |
| 2 | **Cumulative Analysis** | Builds running totals and moving averages to reveal growth trajectory |
| 3 | **Performance Analysis** | Benchmarks products and customers against averages and targets |
| 4 | **Data Segmentation** | Groups customers and products into meaningful tiers |
| 5 | **Part-to-Whole Analysis** | Measures each product's or category's share of total revenue |
| 6 | **Customer Report** | Consolidated customer KPI view for BI consumption |
| 7 | **Product Report** | Consolidated product KPI view for BI consumption |

---

## ❓ Business Questions Answered

### 👥 Customer Analytics

- Who are the most valuable customers by revenue?
- How recently have customers made a purchase (recency)?
- What is each customer's lifespan and average monthly spend?
- How can customers be segmented by purchasing behavior?

### 📦 Product Analytics

- Which products generate the most revenue and highest sales volume?
- Which products underperform relative to category averages?
- What is the average selling price per product?

### 📈 Sales Analysis

- How does sales performance change over time (monthly/yearly)?
- What are the cumulative revenue trends?
- How is revenue distributed across products and categories?

---

## 📋 Reporting Views

### 👥 Customer Report (`6_report_customers.sql`)

A consolidated view combining customer attributes with calculated KPIs, designed for direct consumption by BI tools.

**Metrics included:**

| Metric | Description |
|--------|-------------|
| Total Orders | Number of distinct orders per customer |
| Total Sales | Cumulative revenue generated |
| Total Quantity | Units purchased across all orders |
| Total Products | Distinct products purchased |
| Customer Lifespan | Days between first and last purchase |
| Recency | Days since last purchase |
| Average Order Value | Revenue per order |
| Average Monthly Spend | Revenue normalized by active months |

**Customer Segments:**

| Segment | Description |
|---------|-------------|
| 🏆 VIP | High-value, frequent buyers |
| 🔄 Regular | Consistent mid-tier customers |
| 🆕 New | Recently acquired customers |

---

### 📦 Product Report (`7_report_products.sql`)

A consolidated view combining product attributes with performance KPIs.

**Metrics included:**

| Metric | Description |
|--------|-------------|
| Total Orders | Number of orders containing this product |
| Total Customers | Distinct customers who purchased |
| Total Sales | Cumulative revenue from this product |
| Total Quantity Sold | Units sold |
| Average Selling Price | Revenue per unit |

**Product Performance Tiers:**

| Tier | Description |
|------|-------------|
| 🟢 High Performer | Above-average revenue contribution |
| 🟡 Mid Performer | Average revenue contribution |
| 🔴 Low Performer | Below-average revenue contribution |

---

## 📁 Project Structure

```
sql-business-analytics-project/
│
├── DataAnalysis/
│   ├── 1_change_over_time_analysis.sql   # Sales trends over months/years
│   ├── 2_cumulative_analysis.sql         # Running totals and moving averages
│   ├── 3_performance_analysis.sql        # Benchmarking against averages
│   ├── 4_data_segmentation.sql           # Customer and product tiering
│   ├── 5_part_to_whole_analysis.sql      # Revenue share by product/category
│   ├── 6_report_customers.sql            # Customer KPI reporting view
│   └── 7_report_products.sql             # Product KPI reporting view
│
└── README.md
```

---

## 💡 Skills Demonstrated

- 📐 **Analytical SQL** — Window functions, CTEs, aggregations, and CASE logic across all modules
- 👥 **Customer Segmentation** — RFM-style behavioral tiering (recency, frequency, monetary value)
- 📦 **Product Analytics** — Performance benchmarking and category-level contribution analysis
- 📈 **Trend Analysis** — Time-series breakdowns with running totals and moving averages
- 📊 **KPI Development** — Designed business-ready metrics for executive reporting
- 🗂️ **Reporting Design** — Built reusable views structured for BI tool consumption

---

## 👤 About This Project & Author

**Mersad** — Civil Engineer transitioning into Data Analytics.
Built as part of a self-directed portfolio to demonstrate end-to-end data analytics skills.

This project was designed and built independently to demonstrate practical skills in analytical SQL, customer and product intelligence, and reporting design. It sits on top of a purpose-built Data Warehouse, simulating the kind of analytics layer a BI analyst or data analyst would own in a real business environment.

🔗 [GitHub Portfolio](https://github.com/Mersad-MAZ)
