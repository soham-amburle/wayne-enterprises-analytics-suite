# Wayne Enterprises Security & Risk Management

**Organization:** Wayne Enterprises (Fictional Enterprise Business Model)

**Tool:** Power BI

**Dataset:** Synthetic Enterprise Business Intelligence Dataset – ~100,000 Records

**Dashboard Focus:** Security & Risk Management, Contract Risk, Security Incidents, Regional Risk, Mission Performance & Supply Chain Risk

**Date:** 12 – 19 July 2026

**Created by:** Soham S. Amburle

---

## Overview

The **Wayne Enterprises Security & Risk Management Dashboard** provides an analytical view of enterprise-wide security exposure and operational risk across defense contracts, security incidents, Bat-Tech operations, and supply-chain activities.

Designed using a large-scale synthetic enterprise dataset, this dashboard simulates the security and risk management environment surrounding Wayne Enterprises and provides a centralized platform for monitoring potential vulnerabilities, evaluating risk exposure, analyzing security incidents, and identifying operational areas requiring further investigation.

The dashboard enables executives, security teams, intelligence analysts, risk managers, business analysts, and operational decision-makers to evaluate contractual risk, monitor security incidents, assess incident severity, analyze regional risk concentration, evaluate mission performance, and monitor supply-chain disruptions.

The dashboard focuses on understanding:

* Overall defense contract risk exposure
* High-risk defense contracts
* Total security incident activity
* Critical security incidents
* Security incident resolution performance
* Average incident response time
* Supply-chain delays
* Bat-Tech mission failures
* Risk exposure across different clients
* Security incident distribution across crime types
* Geographic concentration of security incidents
* Mission performance across different mission types
* Regional supply-chain disruption

By combining KPI cards, contract-risk analysis, security incident analytics, regional analysis, mission performance, supply-chain analysis, and interactive filtering capabilities, the dashboard provides a focused enterprise solution for evaluating Wayne Enterprises' security and risk environment.

This dashboard answers several strategic security and risk questions:

* What is the overall average risk score across defense contracts?
* How many defense contracts are classified as high risk?
* How many security incidents have been recorded?
* How many critical security incidents have occurred?
* What percentage of security incidents have been resolved?
* What is the average response time to security incidents?
* What percentage of shipments are affected by delays?
* How frequently do Bat-Tech mission failures occur?
* Which clients have the highest average contract risk?
* Which crime types account for the greatest number of security incidents?
* Which regions have the highest concentration of security incidents?
* How does mission performance vary across different mission types?
* Which regions demonstrate greater supply-chain disruption?

Through KPI cards, analytical visuals, and interactive filtering, the dashboard provides a centralized view of Wayne Enterprises' security exposure and risk environment.

---

## Business Storyline & Analytical Flow

### 1. Security & Risk KPI Snapshot – KPI Cards

Eight KPI cards provide an executive summary of Wayne Enterprises' security and risk environment:

* **AVG RISK SCORE**
* **HIGH-RISK CONTRACTS**
* **SECURITY INCIDENTS**
* **CRITICAL INCIDENTS**
* **RESOLUTION RATE**
* **AVG RESPONSE TIME**
* **SUPPLY DELAYS**
* **MISSION FAILURES**

These KPIs allow executives, security teams, intelligence analysts, and risk managers to quickly assess contractual risk exposure, security incident activity, incident severity, response and resolution performance, supply-chain disruption, and Bat-Tech operational performance.

---

### 2. Security, Contract & Operational Risk Analytics

Five analytical visuals provide deeper insights into Wayne Enterprises' security and risk environment:

1. **RISK BY CLIENT** – Clustered Bar Chart
2. **INCIDENTS BY TYPE** – Stacked Column Chart
3. **REGIONAL RISK** – Bar Chart
4. **MISSION SUCCESS** – Stacked Column Chart
5. **SUPPLY CHAIN RISK** – Clustered Column Chart

These visuals help identify:

* Clients associated with higher average contract risk
* Crime types contributing most significantly to security incidents
* Regional concentrations of security incidents
* Distribution of security incidents across different severity levels
* Successful and unsuccessful Bat-Tech missions
* Mission types with greater operational activity
* Regional supply-chain disruption
* Differences between delayed and non-delayed shipments
* Areas requiring additional security or risk investigation

The combination of contractual, security, geographic, operational, and supply-chain analysis provides a broader view of enterprise risk than incident-level analysis alone.

---

### 3. Interactive Slicers

Seven slicers allow dynamic exploration of Wayne Enterprises' security and risk environment:

* Date (`Dim_Date[Date]`)
* Region (`Dim_Region[Region_Type]`)
* Crime Type (`Fact_CrimeData[Crime_Type]`)
* Severity (`Fact_CrimeData[Severity]`)
* Mission Type (`Fact_BatOperations[Mission_Type]`)
* Client Industry (`Dim_Client[Industry]`)
* Delay Status (`Fact_SupplyChain[Delay_Flag]`)

These filters allow users to analyze security and risk activity across different time periods, regional classifications, crime categories, severity levels, mission types, client industries, and supply-chain delay conditions.

All dashboard visuals dynamically respond to slicer selections, enabling users to move from a broad enterprise risk overview toward more focused security investigations.

---

## Key Insights Enabled by the Dashboard

The dashboard enables executives and business analysts to:

* Monitor overall defense contract risk exposure
* Identify high-risk defense contracts
* Monitor total security incident activity
* Identify critical security incidents
* Evaluate security incident resolution rates
* Monitor average security incident response time
* Identify regions with higher security incident concentrations
* Compare security incidents across different crime types
* Evaluate the severity composition of security incidents
* Compare risk exposure across different clients
* Evaluate Bat-Tech mission performance
* Identify mission failures across different mission types
* Monitor regional supply-chain disruption
* Compare delayed and non-delayed shipments
* Identify operational areas requiring additional risk investigation
* Support data-driven security planning
* Support enterprise risk monitoring and analysis
* Provide a centralized view of internal and external security exposure

---

## Tools & Data

* **Visualization Tool:** Power BI
* **Dataset:** Synthetic enterprise business intelligence dataset
* **Record Count:** ~100,000 records across all tables
* **Model Design:** Hybrid Star Schema
* **Purpose:** Enterprise Business Intelligence portfolio project simulating Wayne Enterprises' security monitoring, contractual risk assessment, criminal intelligence, Bat-Tech operational security, regional risk analysis, and supply-chain risk management

### Tables Used

**Fact Tables**

* Fact_DefenseContracts
* Fact_CrimeData
* Fact_BatOperations
* Fact_SupplyChain

**Dimension Tables**

* Dim_Date
* Dim_Region
* Dim_Client
* Dim_Product

---

## Security & Risk Management Data Structure

The Security & Risk Management Dashboard primarily uses defense contract, security incident, Bat-Tech mission, and supply-chain data, supported by related date, regional, client, and product dimensions.

### Fact_DefenseContracts

The table contains the following contractual risk fields:

* **Contract_ID** – Unique identifier for each defense contract
* **Client_ID** – Reference to the client associated with the contract
* **Start_Date** – Contract start date
* **End_Date** – Contract end date
* **Contract_Value** – Total value of the defense contract
* **Cost** – Cost associated with fulfilling the contract
* **Profit** – Profit generated from the contract
* **Risk_Score** – Risk score associated with the contract
* **Completion_Status** – Current completion status of the contract

### Fact_CrimeData

The table contains the following security incident fields:

* **Incident_ID** – Unique identifier for each security incident
* **Date_ID** – Reference to the incident date
* **Region_ID** – Reference to the geographic region associated with the incident
* **Crime_Type** – Type of security incident recorded
* **Severity** – Severity level of the incident
* **Response_Time** – Response time measured in minutes
* **Resolved_Flag** – Indicates whether the incident was resolved

### Fact_BatOperations

The table contains the following specialized operational security fields:

* **Mission_ID** – Unique identifier for each Bat-Tech mission
* **Date_ID** – Reference to the mission date
* **Product_ID** – Reference to the Bat-Tech asset or product used
* **Mission_Type** – Type of mission conducted
* **Location** – Location associated with the mission
* **Response_Time** – Mission response time
* **Success_Flag** – Indicates whether the mission was successful
* **Threat_Level** – Threat level associated with the mission

### Fact_SupplyChain

The table contains the following supply-chain risk fields:

* **Shipment_ID** – Unique identifier for each shipment
* **Date_ID** – Reference to the shipment date
* **Supplier_Name** – Supplier associated with the shipment
* **Region_ID** – Reference to the shipment region
* **Delivery_Time** – Shipment delivery time
* **Delay_Flag** – Indicates whether the shipment experienced a delay
* **Shipment_Cost** – Cost associated with the shipment
* **Quality_Score** – Quality score associated with the shipment

### Dim_Date

Provides time-related attributes used for temporal analysis and filtering:

* **Date_ID**
* **Date**
* **Day**
* **Month**
* **Month_Name**
* **Quarter**
* **Year**
* **Week_Number**
* **Day_of_Week**
* **Is_Weekend**

### Dim_Region

Provides geographic attributes associated with security and operational analysis:

* **Region_ID**
* **Country**
* **City**
* **Region_Type**
* **Economic_Zone**

### Dim_Client

Provides client-related attributes used for contractual risk analysis:

* **Client_ID**
* **Client_Name**
* **Industry**
* **Contract_Type**
* **Region_ID**
* **Client_Size**

### Dim_Product

Provides product and Bat-Tech asset attributes:

* **Product_ID**
* **Product_Name**
* **Category**
* **Launch_Date**
* **Status**
* **Unit_Cost**

---

## Data Model

The dashboard uses the existing **Hybrid Star Schema** data model.

The primary relationships used by the dashboard are:

* `Dim_Date[Date_ID]` → `Fact_CrimeData[Date_ID]`
* `Dim_Date[Date_ID]` → `Fact_BatOperations[Date_ID]`
* `Dim_Date[Date_ID]` → `Fact_SupplyChain[Date_ID]`
* `Dim_Region[Region_ID]` → `Fact_CrimeData[Region_ID]`
* `Dim_Region[Region_ID]` → `Fact_SupplyChain[Region_ID]`
* `Dim_Client[Client_ID]` → `Fact_DefenseContracts[Client_ID]`
* `Dim_Product[Product_ID]` → `Fact_BatOperations[Product_ID]`

The relationships follow a **one-to-many (1 → *)** structure with **single-direction filtering from the dimension tables to the fact tables**.

No direct fact-to-fact relationships or many-to-many relationships are used within the model.

---

## Data Disclaimer

This dashboard is built using a **synthetic enterprise dataset (~100,000 records)** generated for analytical and demonstration purposes.

The Wayne Enterprises security and risk data simulates fictional defense contracts, security incidents, operational missions, regional risk, and supply-chain activity. It does **not represent real Wayne Enterprises data, real Gotham City security statistics, real defense contracts, or real-world security intelligence**.

The dataset is designed to replicate typical enterprise security and risk analytics scenarios such as:

* Contract risk analysis
* High-risk contract monitoring
* Security incident analysis
* Incident severity analysis
* Response-time analysis
* Resolution performance monitoring
* Regional risk analysis
* Mission performance analysis
* Operational security monitoring
* Supply-chain delay analysis
* Enterprise risk monitoring
* Security intelligence analysis

---

> **Note:** This project is inspired by the fictional enterprise environment of Wayne Enterprises and Gotham City from DC Comics. The security and risk management layer is intentionally designed as a blend of fictional, cinematic, and enterprise business intelligence concepts for portfolio demonstration purposes. All data used in this dashboard is synthetic and created solely for learning, analysis, and portfolio demonstration purposes.

---

**Dashboard and Documentation by SOHAM S. AMBURLE**

**19 July 2026**
