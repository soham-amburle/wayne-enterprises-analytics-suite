# Wayne Enterprises Gotham City Intelligence Analysis Dashboard
 
**Organization:** Wayne Enterprises (Fictional Enterprise Business Model)

**Tool:** Power BI

**Dataset:** Synthetic Enterprise Business Intelligence Dataset – ~100,000 Records

**Dashboard Focus:** Gotham Crime Intelligence, Crime Severity, Resolution Performance, Response Time, Crime Patterns & Geographic Analysis

**Date:** 29 June – 10 July 2026

**Created by:** Soham S. Amburle

---

## Overview

The **Wayne Enterprises Gotham City Intelligence Analysis Dashboard** provides an analytical view of crime activity across Gotham City and other simulated regions, focusing on incident volume, crime severity, resolution performance, response time, crime types, geographic concentration, and crime trends over time.

Designed using a large-scale synthetic enterprise dataset, this dashboard simulates the intelligence and analytical environment surrounding Wayne Enterprises' efforts to understand and monitor criminal activity across Gotham City.

The dashboard enables executives, intelligence analysts, security teams, business analysts, and decision-makers to evaluate crime activity, understand the severity of incidents, monitor resolution performance, analyze response times, and identify geographic and temporal crime patterns.

The dashboard focuses on understanding:

* Total crime incident activity
* Overall crime resolution rate
* High-severity crime incidents
* Average crime response time
* Unresolved crime incidents
* Overall crime severity
* High-severity crime resolution performance
* Crime distribution across different crime types
* Crime concentration across different regions
* Crime severity distribution
* Crime activity trends over time

By combining KPI cards, crime-level analytics, geographic analysis, severity analysis, time-based trends, and interactive filtering capabilities, the dashboard provides a focused intelligence solution for evaluating Gotham City's criminal activity and response performance.

This dashboard answers several strategic intelligence questions:

* How many crime incidents have been recorded?
* What percentage of crime incidents have been resolved?
* How many high-severity incidents have occurred?
* What is the average response time to crime incidents?
* How many crime incidents remain unresolved?
* What is the overall severity level of recorded crime?
* What percentage of high-severity incidents have been resolved?
* Which crime types occur most frequently?
* Which regions have the highest concentration of crime incidents?
* How is crime distributed across different severity levels?
* How does crime activity change over time?

Through KPI cards, analytical visuals, and interactive filtering, the dashboard provides a centralized view of Gotham City's crime intelligence and response performance.

---

## Business Storyline & Analytical Flow

### 1. Gotham City Intelligence KPI Snapshot – KPI Cards

Seven KPI cards provide an executive summary of Gotham City's crime activity and response performance:

* **Total Incidents**
* **Resolution Rate**
* **High-Severity Cases**
* **Avg Response Time**
* **Unresolved Cases**
* **Avg Severity**
* **High-Severity Resolution**

These KPIs allow executives and intelligence teams to quickly assess overall crime volume, resolution effectiveness, threat severity, response performance, unresolved incidents, and high-severity case resolution.

---

### 2. Crime Intelligence & Geographic Analytics

Four analytical visuals provide deeper insights into Gotham City's criminal activity and intelligence patterns:

1. **CRIME TREND** – Line Chart
2. **CRIME BY TYPE** – Clustered Column Chart
3. **CRIME BY REGION** – Bar Chart
4. **SEVERITY DISTRIBUTION** – Donut Chart

These visuals help identify:

* Changes in crime activity over time
* Most frequently occurring crime types
* Geographic concentration of crime incidents
* Distribution of incidents across severity levels
* Periods of increasing or decreasing crime activity
* Differences in crime activity across regions
* Dominant categories of criminal activity
* Areas requiring further intelligence analysis

The combination of crime-volume, crime-type, geographic, severity, and time-series analysis provides a focused view of Gotham City's criminal intelligence environment.

---

### 3. Interactive Slicers

Seven slicers allow dynamic exploration of Gotham City's crime activity:

* Year (`Dim_Date[Year]`)
* Crime Type (`Fact_CrimeData[Crime_Type]`)
* Severity (`Fact_CrimeData[Severity]`)
* City (`Dim_Region[City]`)
* Country (`Dim_Region[Country]`)
* Month (`Dim_Date[Month_Name]`)
* Region Type (`Dim_Region[Region_Type]`)

These filters allow users to analyze crime activity across different time periods, crime categories, severity levels, cities, countries, months, and regional classifications.

---

## Key Insights Enabled by the Dashboard

The dashboard enables executives and business analysts to:

* Monitor overall crime incident activity
* Evaluate crime resolution rates
* Identify high-severity crime incidents
* Monitor average crime response time
* Track unresolved crime cases
* Evaluate overall crime severity
* Assess high-severity case resolution performance
* Compare crime volumes across different crime types
* Identify regions with high concentrations of crime
* Analyze crime distribution across severity levels
* Monitor crime activity trends over time
* Identify periods of increasing or decreasing criminal activity
* Identify geographic crime patterns requiring further investigation
* Support data-driven intelligence and security planning

---

## Tools & Data

* **Visualization Tool:** Power BI
* **Dataset:** Synthetic enterprise business intelligence dataset
* **Record Count:** ~100,000 records across all tables
* **Model Design:** Hybrid Star Schema
* **Purpose:** Enterprise Business Intelligence portfolio project simulating Wayne Enterprises' Gotham City crime intelligence and criminal activity analysis

### Tables Used

**Fact Tables**

* Fact_CrimeData

**Dimension Tables**

* Dim_Date
* Dim_Region

---

## Gotham City Intelligence Data Structure

The Gotham City Intelligence Analysis Dashboard primarily uses crime-level incident data from `Fact_CrimeData`, supported by the related `Dim_Date` and `Dim_Region` dimension tables.

### Fact_CrimeData

The table contains the following crime intelligence fields:

* **Incident_ID** – Unique identifier for each crime incident
* **Date_ID** – Reference to the incident date
* **Region_ID** – Reference to the geographic region associated with the incident
* **Crime_Type** – Type of crime recorded
* **Severity** – Severity level of the incident
* **Response_Time** – Crime response time measured in minutes
* **Resolved_Flag** – Indicates whether the incident was resolved

### Dim_Date

Provides time-related attributes used for temporal analysis and filtering:

* **Date**
* **Month_Name**
* **Quarter**
* **Year**
* Other calendar attributes

### Dim_Region

Provides geographic attributes associated with crime incidents:

* **Region_ID**
* **Country**
* **City**
* **Region_Type**
* **Economic_Zone**

---

## Data Model

The dashboard uses the existing **Hybrid Star Schema** data model.

The primary relationships used by the dashboard are:

* `Dim_Date[Date_ID]` → `Fact_CrimeData[Date_ID]`
* `Dim_Region[Region_ID]` → `Fact_CrimeData[Region_ID]`

Both relationships follow a **one-to-many (1 → *)** structure with **single-direction filtering from the dimension tables to the fact table**.

---

## Data Disclaimer

This dashboard is built using a **synthetic enterprise dataset (~100,000 records)** generated for analytical and demonstration purposes.

The Gotham City crime intelligence data simulates fictional criminal activity, incident severity, response performance, geographic crime patterns, and resolution outcomes. It does **not represent real Wayne Enterprises, real Gotham City crime statistics, or real-world law enforcement data**.

The dataset is designed to replicate typical intelligence and crime analytics scenarios such as:

* Crime volume analysis
* Crime resolution monitoring
* Severity analysis
* Response-time analysis
* Crime-type comparison
* Geographic crime analysis
* Crime trend analysis
* Incident intelligence monitoring
* Regional crime pattern analysis
* Security performance monitoring

---

> **Note:** This project is inspired by the fictional enterprise environment of Wayne Enterprises and Gotham City from DC Comics. The Gotham City intelligence layer is intentionally designed as a blend of fictional and cinematic concepts for business intelligence portfolio demonstration purposes. All data used in this dashboard is synthetic and created solely for learning, analysis, and portfolio demonstration purposes.

---

**Dashboard and Documentation by SOHAM S. AMBURLE**

**10 July 2026**
