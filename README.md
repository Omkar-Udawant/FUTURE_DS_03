# 📊 Marketing Funnel And Conversion Analysis | Power BI

![Power BI](https://img.shields.io/badge/Tool-Power%20BI-yellow)
![Domain](https://img.shields.io/badge/Domain-Data%20Science%20%26%20Analytics-blue)
![Status](https://img.shields.io/badge/Project-Completed-success)
![Internship](https://img.shields.io/badge/Internship-Future%20Interns-purple)

---

## 🚀 Project Overview

This project was developed as part of my **Data Science & Analytics Internship at Future Interns**.  
The objective of this project is to analyze **marketing funnel performance** and evaluate **lead-to-deal conversion efficiency** using an interactive **Power BI dashboard**.

The dashboard focuses on **funnel analysis and conversion storytelling**, helping stakeholders understand how leads move across different funnel stages, where major drop-offs occur, and which marketing channels and lead types contribute most to successful deal conversions. This enables **data-driven optimization of marketing and sales strategies**.

---

## 🛠️ Tools & Technologies

- **Power BI Desktop** – Dashboard design & visualization  
- **DAX (Data Analysis Expressions)** – Funnel KPIs & conversion calculations  
- **Microsoft Excel / CSV** – Dataset handling  
- **Data Modeling** – Relationships & measures  


---


## 🎯 Business Objectives

This dashboard answers key business questions such as:

- How many **total marketing leads** were generated?
- How many leads were **converted into deals**?
- What is the **marketing to deal conversion rate (%)**?
- Where are the **major funnel drop-offs**?
- Which **marketing sources** generate the most leads and won deals?
- Which **lead types** contribute most to successful conversions?
- How do **monthly lead trends** change over time?
- What is the distribution of **won deals by business type**?

---

## 🖼️ Dashboard Pages Overview

### 🔹 Page 1: Marketing Funnel & Conversion Overview

**Purpose:**  
Provides a high-level snapshot of overall marketing performance and funnel efficiency.

**Key KPIs & Visuals:**
- Total Marketing Leads  
- Converted to Deals  
- Won Deals  
- Marketing to Deal Conversion (%)  
- Lead-to-Deal Conversion Funnel  
- Marketing Leads by Source  
- Monthly Marketing Leads Trend  

---

### 🔹 Page 2: Conversion Performance Analysis

**Purpose:**  
Focuses on deep-dive conversion insights across channels, lead types, and business categories.

**Key Visuals:**
- Won Deals by Marketing Source  
- Distribution of Won Deals by Business Type  
- Won Deals by Lead Type (Funnel View)  
- Deal to Won Conversion %  
- Marketing to Deal Conversion %  

---

## 📐 Key DAX Measures Used

```DAX
Total Marketing Leads =
COUNT(marketing_data[lead_id])

Converted Deals =
CALCULATE(
    COUNT(marketing_data[deal_id]),
    marketing_data[deal_status] = "Converted"
)

Won Deals =
CALCULATE(
    COUNT(marketing_data[deal_id]),
    marketing_data[deal_status] = "Won"
)

Marketing to Deal Conversion % =
DIVIDE(
    [Won Deals],
    [Total Marketing Leads],
    0
)
