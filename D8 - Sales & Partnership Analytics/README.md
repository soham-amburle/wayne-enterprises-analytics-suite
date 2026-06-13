# Wayne Enterprises Sales & Partnerships Analytics Dashboard

**Organization:** Wayne Enterprises (Fictional Enterprise Business Model)

**Tool:** Power BI

**Dataset:** Synthetic Enterprise Sales Dataset – ~100,000 Records

**Dashboard Focus:** Sales Performance, Client Partnerships & Product Revenue Analytics

**Date:** 19 May – 24 May 2026

**Created by:** Soham S. Amburle

---

## Overview

The **Sales & Partnerships Analytics Dashboard** provides a comprehensive view of Wayne Enterprises' sales performance, client relationships, product contribution, and revenue generation trends.

Designed using a large-scale synthetic enterprise dataset, this dashboard enables executives, sales leaders, partnership managers, and business analysts to monitor revenue performance, evaluate client portfolios, identify high-performing products, and understand the overall effectiveness of strategic partnerships.

The dashboard consolidates key sales metrics into a centralized analytical platform, allowing decision-makers to identify revenue drivers, evaluate customer segments, and uncover opportunities for future business growth.

The dashboard focuses on understanding:

* Revenue generation trends over time
* Product-level revenue contribution
* Client segment performance
* Partnership effectiveness
* Sales transaction volume
* Product sales distribution
* Revenue concentration across customers
* Business growth opportunities

By combining KPI indicators, performance analytics, product contribution analysis, and interactive filtering capabilities, the dashboard delivers a complete sales intelligence solution for strategic decision-making.

This dashboard answers several strategic questions:

* How much revenue is Wayne Enterprises generating?
* Which products contribute the most to revenue?
* Which client segments generate the highest sales?
* How many sales transactions are being processed?
* What is the average value of each order?
* Which clients represent the strongest partnerships?
* How are products performing relative to sales volume?
* Where should future sales and partnership efforts be focused?

Through KPI cards, analytical visuals, and interactive filtering, the dashboard provides a complete view of Wayne Enterprises' sales ecosystem.

---

## Business Storyline & Analytical Flow

### 1. Sales KPI Snapshot – KPI Cards

Eight KPI cards provide an executive summary of overall sales performance:

* **Total Revenue**
* **Units Sold**
* **Orders**
* **Average Order Value**
* **Average Discount %**
* **Clients**
* **Products**
* **Top Client**

These KPIs allow executives to quickly assess revenue performance, transaction activity, client portfolio strength, product reach, and overall sales effectiveness.

---

### 2. Sales & Partnership Performance Visuals

Four analytical visuals provide deeper insights into revenue generation, product contribution, and client performance:

1. **REVENUE TREND OVER TIME** – Line Chart
2. **PRODUCT REVENUE CONTRIBUTION** – Donut Chart
3. **CLIENT SEGMENT PERFORMANCE** – Clustered Column Chart
4. **PRODUCT PERFORMANCE ANALYSIS** – Scatter Chart

These visuals help identify:

* Revenue growth and seasonality trends
* Product contribution to total revenue
* High-performing client industries
* Revenue distribution across customer segments
* Product sales efficiency
* High-volume versus high-value products
* Strategic partnership opportunities
* Business growth patterns

---

### 3. Interactive Slicers

Seven slicers allow dynamic exploration of sales performance:

* Year (`Dim_Date[Year]`)
* Quarter (`Dim_Date[Quarter]`)
* Month (`Dim_Date[Month_Name]`)
* Client Name (`Dim_Client[Client_Name]`)
* Client Size (`Dim_Client[Client_Size]`)
* Product Name (`Dim_Product[Product_Name]`)
* Industry (`Dim_Client[Industry]`)

These filters enable users to analyze sales performance across multiple time periods, products, clients, and business segments.

---

## Key Insights Enabled by the Dashboard

The dashboard enables executives and analysts to:

* Monitor enterprise-wide sales performance
* Identify top-performing products
* Analyze client segment contribution
* Evaluate strategic partnerships
* Track revenue growth trends
* Understand sales volume distribution
* Optimize customer acquisition strategies
* Support data-driven sales decision-making

---

## Tools & Data

* **Visualization Tool:** Power BI
* **Dataset:** Synthetic enterprise sales dataset
* **Record Count:** ~100,000 records across all tables
* **Model Design:** Hybrid Star Schema
* **Purpose:** Enterprise Business Intelligence portfolio project simulating sales management, partnership analytics, and revenue performance monitoring

### Tables Used

**Fact Tables**

* Fact_Sales

**Dimension Tables**

* Dim_Date
* Dim_Product
* Dim_Client

---

## Data Disclaimer

This dashboard is built using a **synthetic enterprise dataset (~100,000 records)** generated for analytical and demonstration purposes. The data simulates enterprise-level sales operations, client relationship management, product sales performance, and revenue analytics scenarios and does **not represent real corporate sales data**.

The dataset follows a **Hybrid Star Schema data model** consisting of multiple fact tables and dimension tables designed to simulate real-world business intelligence environments.

The data was generated to replicate typical sales analytics scenarios such as:

* Revenue performance analysis
* Product contribution tracking
* Client portfolio evaluation
* Customer segmentation analysis
* Sales trend monitoring
* Order value assessment
* Partnership performance measurement
* Strategic sales decision support

---

> **Note:** This project is inspired by the fictional enterprise environment of Wayne Enterprises from DC Comics. All data used in this dashboard is synthetic and created solely for learning, analysis, and portfolio demonstration purposes.

---

**Dashboard and Documentation by SOHAM S. AMBURLE**
**24 May 2026**
