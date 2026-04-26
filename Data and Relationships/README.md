## 🗃️ Data Model & Table Structure
 
This project follows a **Hybrid Star Schema** approach, combining the performance benefits of a star schema with selective normalization for complex dimensions.

---

# 🔵 Dimension Tables

## 1. Dim_Date

**Purpose:** Central time dimension for all dashboards

| Column Name     | Description |
|----------------|------------|
| Date_ID (PK)   | Unique date key (YYYYMMDD) |
| Date           | Full date |
| Day            | Day of month |
| Month          | Month number |
| Month_Name     | Month name |
| Quarter        | Quarter (Q1–Q4) |
| Year           | Year |
| Week_Number    | Week of year |
| Day_of_Week    | Day name |
| Is_Weekend     | Yes/No flag |

---

## 2. Dim_Department

| Column Name        | Description |
|-------------------|------------|
| Department_ID (PK)| Unique department ID |
| Department_Name   | Name of department |
| Division_Type     | Corporate / Confidential / Hybrid |
| Head_of_Department| Department head |
| Budget_Allocation | Allocated budget |

---

## 3. Dim_Region

| Column Name     | Description |
|----------------|------------|
| Region_ID (PK) | Unique region ID |
| Country        | Country name |
| City           | City (includes Gotham) |
| Region_Type    | Domestic / International |
| Economic_Zone  | Business classification |

---

## 4. Dim_Employee

| Column Name         | Description |
|--------------------|------------|
| Employee_ID (PK)   | Unique employee ID |
| Employee_Name      | Name |
| Department_ID (FK) | Linked department |
| Role               | Job role |
| Experience_Level   | Junior / Mid / Senior |
| Hire_Date          | Joining date |
| Salary_Band        | Salary category |
| Performance_Rating | Performance score |

---

## 5. Dim_Product_Asset

| Column Name     | Description |
|----------------|------------|
| Product_ID (PK)| Unique ID |
| Product_Name   | Name |
| Category       | Commercial / Defense / Bat-Tech |
| Launch_Date    | Launch date |
| Status         | Active / Discontinued / Prototype |
| Unit_Cost      | Cost per unit |

---

## 6. Dim_Client

| Column Name         | Description |
|--------------------|------------|
| Client_ID (PK)     | Unique client ID |
| Client_Name        | Name |
| Industry           | Industry type |
| Contract_Type      | Government / Private |
| Region_ID (FK)     | Linked region |
| Client_Size        | Small / Medium / Enterprise |

---

# 🔴 Fact Tables

## 1. Fact_Finance

| Column Name          | Description |
|---------------------|------------|
| Transaction_ID (PK) | Unique transaction ID |
| Date_ID (FK)        | Date reference |
| Department_ID (FK)  | Department reference |
| Revenue             | Revenue generated |
| Cost                | Cost incurred |
| Profit              | Net profit |
| Investment_Amount   | Investment value |
| ROI                 | Return on investment |

---

## 2. Fact_Sales

| Column Name           | Description |
|----------------------|------------|
| Sales_ID (PK)        | Unique sales ID |
| Date_ID (FK)         | Date reference |
| Product_ID (FK)      | Product reference |
| Client_ID (FK)       | Client reference |
| Revenue              | Sales revenue |
| Units_Sold           | Quantity sold |
| Discount_Percentage  | Discount applied |
| Sales_Channel        | Online / Direct / Partner |

---

## 3. Fact_Operations

| Column Name        | Description |
|-------------------|------------|
| Operation_ID (PK) | Unique operation ID |
| Date_ID (FK)      | Date reference |
| Region_ID (FK)    | Region reference |
| Department_ID (FK)| Department reference |
| Operational_Cost  | Cost |
| Delay_Time        | Delay in hours |
| Efficiency_Score  | 0–100 score |
| Output_Volume     | Production output |

---

## 4. Fact_Marketing

| Column Name      | Description |
|-----------------|------------|
| Campaign_ID (PK)| Campaign ID |
| Date_ID (FK)    | Date reference |
| Channel         | Social / TV / Digital / Events |
| Campaign_Type   | Campaign category |
| Spend           | Marketing spend |
| Impressions     | Reach |
| Clicks          | Click count |
| Conversions     | Conversions |
| Engagement_Rate | Engagement metric |

---

## 5. Fact_HR

| Column Name        | Description |
|-------------------|------------|
| Record_ID (PK)    | Unique record ID |
| Employee_ID (FK)  | Employee reference |
| Date_ID (FK)      | Date reference |
| Attrition_Flag    | Yes/No |
| Performance_Score | Performance |
| Training_Hours    | Training time |
| Promotion_Flag    | Yes/No |
| Absenteeism_Days  | Days absent |

---

## 6. Fact_RnD

| Column Name           | Description |
|----------------------|------------|
| Project_ID (PK)      | Project ID |
| Department_ID (FK)   | Department reference |
| Start_Date           | Start date |
| End_Date             | End date |
| Investment           | Investment |
| Stage                | Research / Prototype / Production |
| Success_Probability  | % likelihood |
| Expected_ROI         | Expected return |
| Actual_Outcome       | Success / Failure / Ongoing |

---

## 7. Fact_DefenseContracts

| Column Name         | Description |
|--------------------|------------|
| Contract_ID (PK)   | Contract ID |
| Client_ID (FK)     | Client reference |
| Start_Date         | Start date |
| End_Date           | End date |
| Contract_Value     | Total value |
| Cost               | Cost |
| Profit             | Profit |
| Risk_Score         | 0–100 |
| Completion_Status  | Completed / Ongoing / Delayed |

---

## 8. Fact_BatOperations

| Column Name      | Description |
|-----------------|------------|
| Mission_ID (PK) | Mission ID |
| Date_ID (FK)    | Date reference |
| Product_ID (FK) | Asset used |
| Mission_Type    | Surveillance / Combat / Rescue |
| Location        | Gotham zones |
| Response_Time   | Minutes |
| Success_Flag    | Yes/No |
| Threat_Level    | Low / Medium / High |

---

## 9. Fact_CrimeData

| Column Name      | Description |
|-----------------|------------|
| Incident_ID (PK)| Incident ID |
| Date_ID (FK)    | Date reference |
| Region_ID (FK)  | Region reference |
| Crime_Type      | Type of crime |
| Severity        | Low / Medium / High |
| Response_Time   | Minutes |
| Resolved_Flag   | Yes/No |

---

## 10. Fact_SupplyChain

| Column Name     | Description |
|----------------|------------|
| Shipment_ID (PK)| Shipment ID |
| Date_ID (FK)   | Date reference |
| Supplier_Name  | Supplier |
| Region_ID (FK) | Region reference |
| Delivery_Time  | Days |
| Delay_Flag     | Yes/No |
| Shipment_Cost  | Cost |
| Quality_Score  | 0–100 |

---

# 🔗 Relationships

All relationships follow a **one-to-many (1 → *) structure** with **single-direction filtering (Dimension → Fact)**.

---

## Dim_Date Relationships

- Dim_Date[Date_ID] → Fact_Sales[Date_ID]  
- Dim_Date[Date_ID] → Fact_Finance[Date_ID]  
- Dim_Date[Date_ID] → Fact_Operations[Date_ID]  
- Dim_Date[Date_ID] → Fact_Marketing[Date_ID]  
- Dim_Date[Date_ID] → Fact_HR[Date_ID]  
- Dim_Date[Date_ID] → Fact_CrimeData[Date_ID]  
- Dim_Date[Date_ID] → Fact_BatOperations[Date_ID]  
- Dim_Date[Date_ID] → Fact_SupplyChain[Date_ID]  

---

## Dim_Department Relationships

- Dim_Department[Department_ID] → Fact_Finance[Department_ID]  
- Dim_Department[Department_ID] → Fact_Operations[Department_ID]  
- Dim_Department[Department_ID] → Fact_RnD[Department_ID]  

---

## Dim_Region Relationships

- Dim_Region[Region_ID] → Fact_Operations[Region_ID]  
- Dim_Region[Region_ID] → Fact_CrimeData[Region_ID]  
- Dim_Region[Region_ID] → Fact_SupplyChain[Region_ID]  

---

## Dim_Employee Relationships

- Dim_Employee[Employee_ID] → Fact_HR[Employee_ID]  

---

## Dim_Product_Asset Relationships

- Dim_Product_Asset[Product_ID] → Fact_Sales[Product_ID]  
- Dim_Product_Asset[Product_ID] → Fact_BatOperations[Product_ID]  

---

## Dim_Client Relationships

- Dim_Client[Client_ID] → Fact_Sales[Client_ID]  
- Dim_Client[Client_ID] → Fact_DefenseContracts[Client_ID]  

---

## Relationship Notes

- No direct relationships between fact tables  
- No many-to-many relationships used  
- All joins are based on surrogate keys (IDs)  
- Model optimized for performance and scalability in Power BI  

---

# 🔢 Data Volume Strategy (~100K Records)

| Table              | Records |
|-------------------|--------|
| Fact_Sales        | 25,000 |
| Fact_CrimeData    | 20,000 |
| Fact_Operations   | 15,000 |
| Fact_Finance      | 10,000 |
| Fact_Marketing    | 8,000  |
| Fact_HR           | 7,000  |
| Fact_RnD          | 5,000  |
| Fact_Defense      | 4,000  |
| Fact_SupplyChain  | 4,000  |
| Fact_BatOperations| 2,000  |

---

## ⚠️ Note

All data is synthetic and designed to simulate realistic enterprise and city-level analytics scenarios.
