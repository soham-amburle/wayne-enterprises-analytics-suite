# Wayne Enterprises Wayne Tech Product Performance Dashboard

**Organization:** Wayne Enterprises (Fictional Enterprise Business Model)

**Tool:** Power BI

**Dataset:** Synthetic Enterprise Business Intelligence Dataset – ~100,000 Records

**Dashboard Focus:** Wayne Tech Product Performance, Sales, Revenue, Profitability & Product Portfolio Analytics

**Date:** 10 June – 16 June 2026

**Created by:** Soham S. Amburle

---

## Overview

The **Wayne Tech Product Performance Dashboard** provides a comprehensive analytical view of Wayne Enterprises' product portfolio, focusing on product sales, revenue generation, sales volume, profitability, client contribution, and product category performance.

Designed using a large-scale synthetic enterprise dataset, this dashboard enables executives, product managers, sales teams, business analysts, and decision-makers to evaluate the commercial performance of Wayne Tech products and understand how different products contribute to the organization's overall revenue and profitability.

The dashboard consolidates key product and sales metrics into a centralized business intelligence platform, allowing decision-makers to understand product performance across clients, industries, client segments, regions, and time periods.

The dashboard focuses on understanding:

* Product revenue performance
* Product sales volume
* Product portfolio composition
* Revenue contribution by product category
* Client contribution to product sales
* Product performance across different industries
* Product profitability
* Pricing and discount behavior
* Revenue trends over time
* Commercial performance across regions

By combining KPI indicators, product performance analytics, revenue composition analysis, time-based trends, and interactive filtering capabilities, the dashboard provides a focused product intelligence solution for strategic commercial decision-making.

This dashboard answers several strategic questions:

* Which Wayne Tech products generate the highest revenue?
* Which products have the highest sales volume?
* Which product categories contribute the most revenue?
* How profitable is the Wayne Tech product portfolio?
* What is the average selling price across products?
* How much discount is being applied to product sales?
* Which clients and industries contribute most to product revenue?
* How does product revenue change over time?
* How does product performance vary across different regions?
* Which areas of the Wayne Tech portfolio require greater commercial attention?

Through KPI cards, analytical visuals, and interactive filtering, the dashboard provides a comprehensive view of Wayne Tech's commercial product ecosystem.

---

## Business Storyline & Analytical Flow

### 1. Product Performance KPI Snapshot – KPI Cards

Eight KPI cards provide an executive summary of Wayne Tech's product sales and financial performance:

* **Total Revenue**
* **Total Units Sold**
* **Total Products Sold**
* **Total Clients**
* **Average Selling Price**
* **Average Discount**
* **Total Profit**
* **Profit Margin**

These KPIs allow executives to quickly assess overall product revenue, sales volume, customer reach, pricing, discount levels, profitability, and product portfolio performance.

---

### 2. Product Sales & Revenue Analytics

Four analytical visuals provide deeper insights into Wayne Tech's product performance and commercial trends:

1. **PRODUCT REVENUE PERFORMANCE** – Clustered Bar Chart
2. **PRODUCT SALES VOLUME** – Clustered Column Chart
3. **REVENUE MIX BY CATEGORY** – Donut Chart
4. **REVENUE TREND** – Line Chart

These visuals help identify:

* Highest-revenue Wayne Tech products
* Highest-volume products
* Revenue concentration across product categories
* Commercial strength of different product segments
* Monthly revenue patterns
* Product portfolio performance over time
* Differences between high-volume and high-value products
* Areas of the portfolio requiring further commercial analysis

The combination of revenue and sales-volume analysis also helps distinguish between products that generate high revenue through premium pricing and products that generate revenue primarily through higher sales volume.

---

### 3. Interactive Slicers

Seven slicers allow dynamic exploration of Wayne Tech product performance:

* Product (`Dim_Product[Product_Name]`)
* Category (`Dim_Product[Category]`)
* Client (`Dim_Client[Client_Name]`)
* Industry (`Dim_Client[Industry]`)
* Client Size (`Dim_Client[Client_Size]`)
* Region (`Dim_Region[City]`)
* Year (`Dim_Date[Year]`)

These filters allow users to analyze product performance across different product categories, clients, industries, client segments, geographic markets, and time periods.

---

## Key Insights Enabled by the Dashboard

The dashboard enables executives and business analysts to:

* Monitor Wayne Tech product revenue performance
* Identify the highest-performing products
* Compare product sales volumes
* Analyze revenue contribution by product category
* Evaluate overall product profitability
* Monitor average selling prices and discount levels
* Understand client and industry contribution
* Analyze regional product performance
* Identify revenue trends over time
* Support product portfolio and commercial strategy decisions
* Enable data-driven product management and sales planning

---

## Tools & Data

* **Visualization Tool:** Power BI
* **Dataset:** Synthetic enterprise business intelligence dataset
* **Record Count:** ~100,000 records across all tables
* **Model Design:** Hybrid Star Schema
* **Purpose:** Enterprise Business Intelligence portfolio project simulating Wayne Enterprises' product sales, revenue, profitability, client, and commercial performance analytics

### Tables Used

**Fact Tables**

* Fact_Sales

**Dimension Tables**

* Dim_Date
* Dim_Product
* Dim_Client
* Dim_Region

---

## Data Disclaimer

This dashboard is built using a **synthetic enterprise dataset (~100,000 records)** generated for analytical and demonstration purposes. The data simulates enterprise-level product sales, commercial performance, client activity, product portfolio management, pricing, and profitability scenarios and does **not represent real Wayne Enterprises or real-world commercial data**.

The dataset follows a **Hybrid Star Schema data model** consisting of multiple fact tables and dimension tables designed to simulate real-world business intelligence environments.

The data was generated to replicate typical product and commercial analytics scenarios such as:

* Product revenue analysis
* Sales volume monitoring
* Product portfolio analysis
* Revenue contribution analysis
* Client segmentation
* Industry-level sales analysis
* Regional product performance
* Pricing and discount analysis
* Profitability assessment
* Commercial performance monitoring

---

> **Note:** This project is inspired by the fictional enterprise environment of Wayne Enterprises from DC Comics. All data used in this dashboard is synthetic and created solely for learning, analysis, and portfolio demonstration purposes.

---

**Dashboard and Documentation by SOHAM S. AMBURLE**
**16 June 2026**
