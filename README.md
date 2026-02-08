🏦 Bank Customer Churn Analysis

_A data-driven analysis project focused on identifying customer churn drivers and building actionable retention strategies for a retail banking environment using Power BI._

---

## 📌 Table of Contents
- [Overview](#overview)  
- [Business Problem](#business-problem)  
- [Dataset](#dataset)  
- [Tools & Technologies](#tools--technologies)  
- [Project Structure](#project-structure)  
- [Data Cleaning & Preparation](#data-cleaning--preparation)  
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)  
- [Research Questions & Key Findings](#research-questions--key-findings)  
- [Dashboard](#dashboard)  
- [Final Recommendations](#final-recommendations)

---

## Overview 
Customer churn is one of the most critical problems in the banking industry. Retaining existing customers is significantly cheaper than acquiring new ones, yet many banks are unable to identify early warning signals before a customer leaves.

This project analyzes customer demographics, activity behavior, financial attributes, and product usage patterns to uncover why customers churn and which customer segments are most at risk.
An interactive Power BI dashboard is built to make churn analysis intuitive and decision-ready for business stakeholders.

---

## Business Problem

The bank is experiencing consistent customer attrition, which leads to:
- Loss of revenue
- Reduction in deposits
- Higher customer acquisition costs
- Weakened customer lifetime value (LTV)

### The business needs to know:
- Why are customers leaving?
- Which customers are most likely to churn?
- What behaviors indicate churn risk?
- Which customers should be prioritized for retention?

Without deep churn insight, marketing campaigns remain generic and ineffective.

---

## Dataset

### Source
Internal HR dataset provided as:
- `Bank Customer Churn Prediction.csv` (raw data)
- `Cleaned_dataset.csv` (processed version for analysis)

### Size
- **10,000 customer records**

### Key Columns:

| Column          | Description                       |
| --------------- | --------------------------------- |
| CustomerId      | Unique customer identifier        |
| CreditScore     | Credit score of customer          |
| Geography       | Country (France, Germany, Spain)  |
| Gender          | Male / Female                     |
| Age             | Customer age                      |
| Tenure          | Years with bank                   |
| Balance         | Account balance                   |
| NumOfProducts   | Number of financial products      |
| HasCrCard       | Credit card ownership             |
| IsActiveMember  | Customer activity status          |
| EstimatedSalary | Annual income                     |
| Exited          | Churn flag (1 = Left, 0 = Stayed) |

---

## Tools and Technologies
- Power BI – Data visualization & dashboard
- Excel – Pre-validation and light data review

---

## Project Structure
```
Bank Customer Churn Analysis Dashboard/
|
├── data/                     # CSV Files
│   ├── cleaned_dataset.csv
│
├── sql/                     # sql Files
│   ├── healthcare.sql
|
├── Power BI Dashboard/       # Power BI dashboard file
│   └── Healthcare Dashboard.pbix
│
├── README.md

```

---

## Data Cleaning & Preparation
The following cleaning steps were performed before dashboard creation:
- Removed duplicate records using CustomerId.
- Validated age ranges.
- Standardized gender and country naming.
- Verified balance and salary fields to eliminate negative values.
- Converted categorical values to consistent formats.
- Ensured churn column is binary.

---

## Exploratory Data Analysis (EDA)

### Key observations:
- Overall churn rate ≈ 20.4%
- France has the most customers.
- Highest customer volume:
   - Age 31–40
   - Credit score 601–700
- Many customers hold:
   - Only one product
- Inactive customers show significantly higher churn.
- Multiple-product customers are more loyal.
- High churn observed in:
   - Certain balance ranges (100k–200k)
   - Mid-tier credit scores

---

## Research Questions & Key Findings

### Q1: What is the churn rate?
- ≈ 20.4%

### Q2: Who churns most?
- Inactive users
- One-product customers
- Certain high-balance customers

### Q3: Does age impact churn?
- Yes. Mid-aged customers drive most churn volume.

### Q4: Does balance indicate loyalty?
- No. High balance does not guarantee retention.

### Q5: Does engagement reduce churn?
- Strongly. Active members churn less.

### Q6: Is product ownership relevant?
- Yes. Customers with multiple products stay longer.

--- 

## Dashboard
The Power BI dashboard includes:
- Churn Overview (Gauge)
- Customers by:
   - Gender
   - Activity Status
   - Geography
   - Product Count
- Churn by:
   - Age Groups
   - Credit Score
   - Balance Buckets

Dashboard file:  
📁 <img width="918" height="518" alt="Churn_Analysis" src="https://github.com/komalb30/Bank-Churn-Analysis/blob/main/dashboard/Churn_Analysis.png" />

---

## Final Recommendations
- High-balance customers
- Inactive customers
- Track campaign success metrics
- Loyalty incentives for long-tenure users



