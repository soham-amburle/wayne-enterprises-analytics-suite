# Wayne Enterprises Global Supply Chain Command Centre

**Organization:** Wayne Enterprises (Fictional Enterprise Business Model)
**Tool:** Power BI
**Dataset:** Synthetic Enterprise Operations Dataset – ~100,000 Records
**Dashboard Focus:** Supply Chain Performance, Logistics Efficiency & Operational Intelligence
**Date:** 28 April – 05 May 2026
**Created by:** Soham S. Amburle

---

## Overview

The **Global Supply Chain Command Centre Dashboard** provides a centralized operational view of Wayne Enterprises' manufacturing, logistics, and supply chain ecosystem.

Designed using a large-scale synthetic enterprise dataset, this dashboard enables executives, operations leaders, logistics managers, and supply chain analysts to monitor shipment performance, operational efficiency, delivery bottlenecks, and regional logistics effectiveness across the organization.

The dashboard combines manufacturing operations and supply chain intelligence into a single command center, allowing decision-makers to identify inefficiencies, reduce delays, optimize operational costs, and improve overall logistics performance.

The dashboard focuses on understanding:

* Global shipment performance across regions
* Operational efficiency across departments
* Delivery time trends and logistics bottlenecks
* Shipment cost distribution across locations
* Regional delay concentration
* Enterprise-wide supply chain health
* Operational cost monitoring
* Manufacturing and logistics efficiency

By combining KPI indicators, operational analytics, regional performance visuals, and interactive filtering capabilities, the dashboard delivers a comprehensive supply chain intelligence solution for strategic decision-making.

This dashboard answers several strategic questions:

* Which regions generate the highest shipment costs?
* Which locations experience the longest delivery times?
* Where are shipment delays occurring most frequently?
* Which departments demonstrate the highest operational efficiency?
* How healthy is the overall supply chain operation?
* Which operational areas require process optimization?
* How do logistics costs vary across regions?
* What operational trends impact enterprise-wide performance?

Through KPI cards, analytical visuals, and interactive filtering, the dashboard provides a complete view of Wayne Enterprises' manufacturing and logistics operations.

---

## Business Storyline & Analytical Flow

### 1. Supply Chain KPI Snapshot – KPI Cards

Eight KPI cards provide an executive summary of overall supply chain performance:

* **Total Shipments**
* **Shipment Cost**
* **Avg Delivery (Days)**
* **Delay Rate**
* **Delays**
* **OP Cost**
* **Efficiency Score**
* **Total Operations**

These KPIs allow executives to quickly assess logistics performance, operational costs, delivery efficiency, and overall supply chain effectiveness.

---

### 2. Manufacturing & Supply Chain Performance Visuals

Five analytical visuals provide deeper insights into regional logistics performance and operational efficiency:

1. **SHIPMENT COST BY REGION** – Clustered Bar Chart
2. **AVG DELIVERY TIME BY REGION** – Clustered Column Chart
3. **EFFICIENCY SCORE BY DEPARTMENT** – Clustered Bar Chart
4. **DELAYED SHIPMENTS BY REGION** – Clustered Bar Chart
5. **OPERATIONAL EFFICIENCY INDEX** – Gauge Chart

These visuals help identify:

* Regions with the highest logistics expenditure
* Locations experiencing delivery bottlenecks
* Operational efficiency across departments
* Areas contributing most to shipment delays
* Overall supply chain performance against target efficiency levels
* Opportunities for logistics optimization and cost reduction

---

### 3. Interactive Slicers

Seven slicers allow dynamic exploration of operational and logistics performance:

* Year (`Dim_Date[Year]`)
* Quarter (`Dim_Date[Quarter]`)
* Month Name (`Dim_Date[Month_Name]`)
* Country (`Dim_Region[Country]`)
* City (`Dim_Region[City]`)
* Department Name (`Dim_Department[Department_Name]`)
* Region Type (`Dim_Region[Region_Type]`)

These filters enable users to analyze shipment activity, operational efficiency, and logistics performance across multiple business dimensions.

---

## Key Insights Enabled by the Dashboard

The dashboard enables executives and analysts to:

* Monitor enterprise-wide shipment performance
* Analyze logistics costs across global regions
* Identify delivery bottlenecks and delay hotspots
* Evaluate operational efficiency across departments
* Track supply chain performance over time
* Assess regional logistics effectiveness
* Improve manufacturing and distribution planning
* Support strategic operational decision-making

---

## Tools & Data

* **Visualization Tool:** Power BI
* **Dataset:** Synthetic enterprise operations dataset
* **Record Count:** ~100,000 records across all tables
* **Model Design:** Hybrid Star Schema
* **Purpose:** Enterprise Business Intelligence portfolio project simulating global manufacturing, logistics, and supply chain analytics

### Tables Used

**Fact Tables**

* Fact_SupplyChain
* Fact_Operations

**Dimension Tables**

* Dim_Date
* Dim_Region
* Dim_Department

---

## Data Disclaimer

This dashboard is built using a **synthetic enterprise dataset (~100,000 records)** generated for analytical and demonstration purposes. The data simulates enterprise-level manufacturing operations, logistics management, and supply chain performance scenarios and does **not represent real corporate operational data**.

The dataset follows a **Hybrid Star Schema data model** consisting of multiple fact tables and dimension tables designed to simulate real-world business intelligence environments.

The data was generated to replicate typical supply chain analytics scenarios such as:

* Shipment performance monitoring
* Logistics cost analysis
* Delivery efficiency tracking
* Regional supply chain performance evaluation
* Operational efficiency measurement
* Enterprise-wide logistics optimization

---

> **Note:** This project is inspired by the fictional enterprise environment of Wayne Enterprises from DC Comics. All data used in this dashboard is synthetic and created solely for learning, analysis, and portfolio demonstration purposes.

---

**Dashboard and Documentation by SOHAM S. AMBURLE**
**05 May 2026**
