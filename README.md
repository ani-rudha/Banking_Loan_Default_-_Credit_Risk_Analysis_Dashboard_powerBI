# 🏦 Banking Loan Default & Credit Risk Analysis Dashboard (Power BI)
This project presents an end-to-end **Banking Loan Performance and Credit Risk Analysis** built using Power BI to identify credit risk patterns, default drivers, repayment behavior, and high risk customer segments

The dashboard integrates default risk analytics, credit risk segment optimization and repayment behavioral analysis to simulate synthetic banking risk analysis with emphasis on loan and credit risks.

---

## ✴️ Project Overview

The objective of this project was to:

- Design a clean star-schema data model
- Implement advanced DAX measures
- Build executive-ready KPI dashboards
- Identify revenue concentration, loan risk and credit risk segment exposure
- Deliver actionable business insights

---

## 🎯 Business Objectives

- Measure overall loan portfolio risk exposure.
- Identify high-risk customer segments and loan types.
- Analyze credit score and utilization impact on default.
- Monitor repayment behavior as an early warning signal.
- Provide actionable insights for underwriting and pricing strategy. 

---

## 📂 Dataset Description

The dataset consists of the following tables:

| Table | Description |
|--------|------------|
| `tab_customers` | Demographics, income, credit score, region|
| `tab_loans` | Loan amount, interest rate, loan type, tenure |
| `tab_defaults` | Default status and default reasons |
| `tab_repayments` | Payment behavior and delay analysis |
| `tab_credit_history` | Prior loans, prior defaults, utilization |
| `MyMeasures` | Dedicated table to store all DAX measures |

---

## 🧱 Data Model Design

The model follows a **star schema structure**:  
- `tab_loans` acts as the central fact table.
- `tab_customers`, `tab_credit_history` act as dimension tables.
- `tab_defaults` and `tab_repayments` extend loan-level performance tracking. 
- Relationships are built using `customer_id` and `loan_id` keys with one-to-many cardinality

This ensures proper filter propagation and KPI accuracy.

---

## 🧮 Key DAX Measures

### Core Financial KPIs
- Average Credit Score
- Average Interest Rate
- Default Rate (%)
- Total Default
- Total Loan Amount 
- Total Loan
- On Time Payment (%)
- Late Payment (%)
- Partial Payment (%)
- Average Delay Days 

### Default and Credit Risk Analysis
- Default Reason Breakdown
- Credit Score Distribution
- Default Rate (%) by Credit Score Band 
- Loan Type vs Credit Score (Matrix)
- Credit Utilization vs Credit Score
- Loan Type v/s Risk Segment (Matrix)
- Default Rate by High Risk Segment
- Prior Defaults Impact

###Repayment Behavior Analysis
- Average Delay by Loan Type
- Late Payment Rate by Loan Type
- Repayment Amount Trend
- Default Type vs Payment Type 

All measures were implemented using proper filter context handling to ensure KPI integrity and prevent row-context distortion.

---

## 📈 Dashboard Structure

### 1️⃣ Executive Summary
- Total Loans  
- Total Loan Amount  
- Total Defaults  
- Default Rate %  
- Average Credit Score  
- Average Interest Rate  

Purpose: Provide a high-level portfolio health snapshot including loan exposure, borrower quality, and overall default risk.

### 2️⃣ Default Risk Segmentation
- Default Rate by Loan Type  
- Default Rate by Region  
- Default Rate by Credit Score Band  
- Default Distribution Matrix  
- Loan Amount Exposure by Risk Segment  

Purpose: Identify high-risk loan categories, regional concentration, and structural default drivers.

### 3️⃣ Credit Risk Drivers Analysis
- Credit Utilization vs Credit Score (Scatter Plot)  
- Loan Amount Exposure by Risk Band  
- Default Distribution by Credit Score Band  
- Risk-Based Color Segmentation  

Purpose: Analyze structural credit risk patterns and detect clusters of high exposure combined with weak borrower profiles.

### 4️⃣ Repayment Behavior Analysis
- On-Time Payment %  
- Late Payment %  
- Partial Payment %  
- Average Delay Days  
- Default vs Late Payment Comparison Matrix  
- Repayment Trend Analysis  

Purpose: Monitor behavioral repayment patterns and evaluate early warning signals of credit deterioration.
                         
### 📝Overall Dashboard Objective
To provide a complete 360° view of credit risk by combining:

- Portfolio Exposure  
- Structural Risk Drivers  
- Segment-Level Default Analysis  
- Behavioral Monitoring Framework  

This enables better underwriting decisions, pricing strategy adjustments, and proactive risk management.

---

## 🎨Advance UX Feartures

- Dynamic slicers (Region, Loan Type, Credit Score Band)  
- Conditional formatting for high-risk segments  
- Risk color rules in scatter plots  
- Drill-through capability to loan level  
- Custom `MyMeasures` table for clean DAX management  
- Consistent risk color theme (Green → Yellow → Red)

The dashboard balances analytical depth with professional presentation design.

---

## 🔍 Key Business Insights

- Total Default is 44 and Total Loan is 800 with $121.13M Loan amount 
- Average Credit Score is around 673.66 and Default Rate is 5.50% 
- Auto loans and the South region show the highest default concentration.
- The Poor credit score segment contributes maximum defaults.
- Credit utilization shows strong correlation with lower credit scores.
- On Time Payment (49.96%) and Late Payment (50.04%) is almost 50-50
- Repayment delay patterns are uniformly distributed (synthetic dataset limitation, not real-world).

---

## 💼 Business Recommendations

- Tighten underwriting for low credit score customers.
- Monitor high utilization customers proactively.
- Introduce early-warning triggers based on repayment delays.
- Reassess pricing strategy for high-risk loan segments.

---

## 🛠 Tools Used

- Power BI  
- Data Modeling (Star Schema Logic)  
- Advanced DAX Measures  
- Power Query (Data Cleaning & Transformation)
- Risk Segmentation Techniques  
- Behavioral Delay Calculations

---

## 🚀 Portfolio Value

This project demonstrates:

- End-to-end BI development 
- Strong data modeling fundamentals
- Advanced DAX implementation
- Risk segmentation logic  
- Behavioral analytics framework  
- Debugging & validation skills  
- Business storytelling approach

Suitable for roles in:

- Credit Risk Analytics  
- Financial Data Analytics  
- Banking BI Analyst  
- Risk & Portfolio Management 

It reflects the ability to move beyond descriptive reporting and deliver actionable operational and financial risk insights.

---
>Note *For any questions or collaboration opportunities, feel free to reach out!*


