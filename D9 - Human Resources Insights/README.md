# Wayne Enterprises Human Resources Insights Dashboard

**Organization:** Wayne Enterprises (Fictional Enterprise Business Model)

**Tool:** Power BI

**Dataset:** Synthetic Enterprise Human Resources Dataset – ~100,000 Records

**Dashboard Focus:** Workforce Performance, Employee Development, Training & Attrition Analytics

**Date:** 25 May – 30 May 2026

**Created by:** Soham S. Amburle

---

## Overview

The **Human Resources Insights Dashboard** provides a comprehensive analytical view of Wayne Enterprises' workforce, employee development initiatives, training effectiveness, performance management, and retention trends.

Designed using a large-scale synthetic enterprise dataset, this dashboard enables HR leaders, department heads, executives, and business analysts to monitor workforce health, evaluate employee performance, assess training investments, and identify retention risks across the organization.

The dashboard consolidates key human resource metrics into a centralized intelligence platform, allowing decision-makers to better understand employee behavior, workforce capability, organizational performance, and talent development outcomes.

The dashboard focuses on understanding:

* Employee workforce distribution
* Performance management effectiveness
* Employee development and training participation
* Workforce retention trends
* High-performer identification
* Experience-level performance analysis
* Employee engagement through training
* Organizational talent management

By combining KPI indicators, workforce analytics, performance analysis, training evaluation, and interactive filtering capabilities, the dashboard delivers a complete human resources intelligence solution for strategic workforce planning.

This dashboard answers several strategic questions:

* How large is the current workforce?
* What is the overall employee performance level?
* How effective are training programs?
* Which employee groups demonstrate the highest performance?
* What percentage of employees are leaving the organization?
* How does experience influence employee performance?
* Are training investments contributing to workforce improvement?
* Which workforce segments require retention focus?

Through KPI cards, analytical visuals, and interactive filtering, the dashboard provides a complete view of Wayne Enterprises' human capital ecosystem.

---

## Business Storyline & Analytical Flow

### 1. Workforce KPI Snapshot – KPI Cards

Eight KPI cards provide an executive summary of workforce performance and employee development:

* **Total Employees**
* **Avg Performance**
* **Attrition Rate %**
* **Training Rate %**
* **Avg Training Hours**
* **Trained Employees**
* **High Performers**
* **Total Training Hours**

These KPIs allow executives to quickly assess workforce size, employee performance, training participation, retention levels, and overall talent development effectiveness.

---

### 2. Workforce Performance & Retention Analytics

Five analytical visuals provide deeper insights into employee performance, development, and workforce retention:

1. **EMPLOYEE DISTRIBUTION BY DEPARTMENT** – Clustered Bar Chart
2. **AVERAGE PERFORMANCE BY EXPERIENCE LEVEL** – Clustered Column Chart
3. **EMPLOYEE DEVELOPMENT FUNNEL** – Funnel Chart
4. **ATTRITION BY EXPERIENCE LEVEL** – Clustered Bar Chart
5. **TRAINING VS PERFORMANCE ANALYSIS** – Scatter Chart

These visuals help identify:

* Workforce allocation across departments
* Performance differences by experience level
* Employee development progression
* Workforce retention patterns
* Attrition concentration areas
* Training participation effectiveness
* Correlation between training and performance
* Talent management opportunities

---

### 3. Interactive Slicers

Seven slicers allow dynamic exploration of workforce performance and employee development metrics:

* Year (`Dim_Date[Year]`)
* Month (`Dim_Date[Month_Name]`)
* Department (`Dim_Department[Department_Name]`)
* Role (`Dim_Employee[Role]`)
* Experience Level (`Dim_Employee[Experience_Level]`)
* Salary Band (`Dim_Employee[Salary_Band]`)
* Performance Rating (`Dim_Employee[Performance_Rating]`)

These filters enable users to analyze workforce trends across multiple employee segments, organizational units, and time periods.

---

## Key Insights Enabled by the Dashboard

The dashboard enables executives and HR leaders to:

* Monitor workforce performance across the organization
* Evaluate employee development initiatives
* Track workforce retention and attrition trends
* Identify high-performing employee groups
* Assess training effectiveness
* Analyze workforce distribution by department
* Support strategic workforce planning
* Enable data-driven talent management decisions

---

## Tools & Data

* **Visualization Tool:** Power BI
* **Dataset:** Synthetic enterprise human resources dataset
* **Record Count:** ~100,000 records across all tables
* **Model Design:** Hybrid Star Schema
* **Purpose:** Enterprise Business Intelligence portfolio project simulating workforce management, employee development, retention analytics, and organizational performance monitoring

### Tables Used

**Fact Tables**

* Fact_HR

**Dimension Tables**

* Dim_Date
* Dim_Employee
* Dim_Department

---

## Data Disclaimer

This dashboard is built using a **synthetic enterprise dataset (~100,000 records)** generated for analytical and demonstration purposes. The data simulates enterprise-level workforce management, employee development, training programs, performance evaluation, and retention monitoring scenarios and does **not represent real employee data**.

The dataset follows a **Hybrid Star Schema data model** consisting of multiple fact tables and dimension tables designed to simulate real-world business intelligence environments.

The data was generated to replicate typical human resources analytics scenarios such as:

* Workforce performance analysis
* Employee retention monitoring
* Attrition trend analysis
* Training effectiveness evaluation
* Employee development tracking
* Talent management assessment
* Workforce planning support
* Organizational performance measurement

---

> **Note:** This project is inspired by the fictional enterprise environment of Wayne Enterprises from DC Comics. All data used in this dashboard is synthetic and created solely for learning, analysis, and portfolio demonstration purposes.

---

**Dashboard and Documentation by SOHAM S. AMBURLE**
**30 May 2026**
