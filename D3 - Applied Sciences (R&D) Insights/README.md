# Wayne Enterprises Applied Sciences Intelligence Suite – R&D & Innovation Analytics

**Organization:** Wayne Enterprises (Fictional Enterprise Business Model)  
**Tool:** Power BI  
**Dataset:** Synthetic Enterprise Operations Dataset – ~100,000 Records  
**Dashboard Focus:** Research & Development Performance, Innovation Efficiency & ROI Analytics  
**Date:** 16 - 19 April 2026  
**Created by:** Soham S. Amburle  

---

## Overview

The **Applied Sciences (R&D) Insights Dashboard** provides a strategic overview of Wayne Enterprises’ research and innovation ecosystem by analyzing R&D investments, project performance, innovation efficiency, success probability, and expected return generation across Applied Sciences initiatives.

Built using a large-scale synthetic enterprise dataset, the dashboard enables executives, innovation leaders, research analysts, and strategic stakeholders to monitor the effectiveness of enterprise R&D operations while identifying high-potential innovation initiatives and resource allocation efficiency.

The dashboard focuses on understanding:

- Overall R&D investment allocation
- Research project performance and lifecycle stages
- Innovation success probability analysis
- Expected ROI generation across projects
- Ongoing vs successful project distribution
- Investment efficiency across Applied Sciences divisions

By combining KPI indicators, investment trend analysis, innovation performance visuals, and interactive filtering capabilities, the dashboard delivers a comprehensive Applied Sciences intelligence view for executive decision-making.

This dashboard answers several strategic questions:

- How much is Wayne Enterprises investing in R&D initiatives?
- Which research stages receive the highest investment?
- Which projects have the highest expected ROI potential?
- What is the overall innovation success rate?
- How are R&D investments evolving over time?
- What percentage of projects are successful, ongoing, or failing?

Through KPI cards, analytical visuals, and interactive filtering, the dashboard provides a complete overview of enterprise innovation performance and Applied Sciences efficiency.

---

## Business Storyline & Analytical Flow

### 1. Applied Sciences KPI Snapshot – KPI Cards

Six KPI cards provide a quick summary of enterprise R&D performance:

- **Total R&D Investment**
- **Total R&D Projects**
- **Average Success Probability**
- **Expected ROI**
- **Active Projects**
- **Success Rate %**

These KPIs allow executives and innovation leaders to quickly evaluate the effectiveness, efficiency, and future potential of Wayne Enterprises’ Applied Sciences division.

---

### 2. R&D Performance & Innovation Analytics Visuals

Four analytical visuals provide deeper insights into research performance, investment distribution, and innovation outcomes:

1. **R&D INVESTMENT BY STAGE** – Clustered Column Chart  
2. **EXPECTED ROI VS SUCCESS PROBABILITY** – Scatter Plot  
3. **PROJECT OUTCOME DISTRIBUTION** – Donut Chart  
4. **R&D INVESTMENT TREND** – Line Chart  

These visuals help identify:

- Investment allocation across research stages
- High-potential innovation initiatives
- Correlation between investment and success probability
- Distribution of successful, ongoing, and failed projects
- Long-term R&D investment trends
- Innovation efficiency and project maturity analysis

---

### 3. Interactive Slicers

Seven slicers allow dynamic filtering across organizational and innovation dimensions:

- Stage (`Fact_RnD[Stage]`)
- Actual Outcome (`Fact_RnD[ACTUAL_OUTCOME]`)
- Department Name (`Dim_Department[Department_Name]`)
- Year (`Dim_Date[Year]`)
- Division Type (`Dim_Department[Division_Type]`)
- Success Probability Range (`Fact_RnD[Success_Probability]`)
- Expected ROI Range (`Fact_RnD[EXPECTED_ROI]`)

These filters enable users to explore Applied Sciences performance across different innovation stages, departments, and investment-performance ranges.

---

## Key Insights Enabled by the Dashboard

The dashboard enables executives and innovation analysts to:

- Monitor enterprise-wide R&D investment performance
- Identify high-potential innovation projects
- Evaluate research effectiveness and innovation success rates
- Compare project outcomes across research stages
- Analyze expected ROI across Applied Sciences initiatives
- Track long-term innovation investment trends
- Understand project lifecycle distribution and operational efficiency

---

## Tools & Data

- **Visualization Tool:** Power BI  
- **Dataset:** Synthetic enterprise operations dataset  
- **Record Count:** ~100,000 records across all tables  
- **Model Design:** Hybrid Star Schema  
- **Purpose:** Enterprise Business Intelligence portfolio project simulating research, innovation, and Applied Sciences analytics  

### Tables Used

**Fact Tables**

- Fact_RnD  

**Dimension Tables**

- Dim_Department  
- Dim_Date  

---

## Data Disclaimer

This dashboard is built using a **synthetic enterprise dataset (~100,000 records)** generated for analytical and demonstration purposes. The data simulates enterprise-level research, innovation, and investment analytics scenarios and does **not represent real corporate or scientific research data**.

The dataset follows a **Hybrid Star Schema data model** consisting of multiple fact tables and dimension tables designed to simulate real-world business intelligence environments.

The data was generated to replicate typical enterprise analytics scenarios such as:

- R&D investment analysis
- Innovation project tracking
- Research stage performance evaluation
- Success probability assessment
- ROI forecasting and efficiency analysis
- Applied Sciences operational monitoring

---

> **Note:** This project is inspired by the fictional enterprise environment of Wayne Enterprises from DC Comics. All data used in this dashboard is synthetic and created solely for learning, analysis, and portfolio demonstration purposes.

---

**Dashboard and Documentation by SOHAM S. AMBURLE**  
**19 April 2026**
