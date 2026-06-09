# SQL Business Analytics Project

## Overview

This project demonstrates business-focused analytics built on top of a SQL Data Warehouse. The analysis transforms raw transactional data into actionable business insights through customer segmentation, product performance evaluation, trend analysis, and reporting views.

The project uses SQL Server and analytical SQL techniques to answer real business questions and support data-driven decision-making.

---

## Objectives

* Analyze customer purchasing behavior.
* Evaluate product performance.
* Measure sales trends over time.
* Create reusable reporting views.
* Generate business-ready KPIs and insights.

---

## Dataset

The analysis is based on a curated Gold Layer from a Data Warehouse integrating CRM and ERP source systems.

Main analytical tables:

* gold.dim_customers
* gold.dim_products
* gold.fact_sales

---

## Project Structure

```text
sql-business-analytics-project/
│
├── Analysis/
│   ├── 1_change_over_time_analysis.sql
│   ├── 2_cumulative_analysis.sql
│   ├── 3_performance_analysis.sql
│   ├── 4_data_segmentation.sql
│   ├── 5_part_to_whole_analysis.sql
│   ├── 6_report_customers.sql
│   └── 7_report_products.sql
│
└── README.md
```

---

## Business Questions Answered

### Customer Analytics

* Who are the most valuable customers?
* Which customers generate the highest revenue?
* How recently have customers purchased?
* What is the customer lifespan?
* How can customers be segmented based on purchasing behavior?

### Product Analytics

* Which products generate the most revenue?
* Which products have the highest sales volume?
* Which products underperform?
* What is the average selling price?

### Sales Analysis

* How does sales performance change over time?
* What are the cumulative sales trends?
* How is revenue distributed across products?

---

## Analytical Techniques Used

### Change Over Time Analysis

Evaluates trends and performance across different time periods.

### Cumulative Analysis

Calculates running totals and cumulative business metrics.

### Performance Analysis

Measures sales effectiveness and business performance indicators.

### Data Segmentation

Groups customers and products into meaningful business categories.

### Part-to-Whole Analysis

Measures contribution percentages across products and categories.

---

## Reporting Views

### Customer Report

Key metrics include:

* Total Orders
* Total Sales
* Total Quantity Purchased
* Total Products Purchased
* Customer Lifespan
* Recency
* Average Order Value
* Average Monthly Spend

Customer Segments:

* VIP
* Regular
* New

### Product Report

Key metrics include:

* Total Orders
* Total Customers
* Total Sales
* Total Quantity Sold
* Average Selling Price

Product Categories:

* High Performer
* Mid Performer
* Low Performer

---

## Technologies Used

* SQL Server
* T-SQL
* Window Functions
* Aggregations
* Common Table Expressions (CTEs)
* Analytical SQL Queries

---

## Skills Demonstrated

* Business Analytics
* Customer Segmentation
* Product Analytics
* KPI Development
* Sales Analysis
* Data Storytelling
* Reporting Design
* Advanced SQL

---

## Future Improvements

* Power BI Dashboard Integration
* Predictive Customer Segmentation
* Sales Forecasting
* Automated Reporting Pipelines

---

## Author

Created as a personal portfolio project to demonstrate SQL-based business analytics and reporting capabilities.
