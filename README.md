# 📊 Marketing Funnel And Conversion Analysis | Power BI

![Power BI](https://img.shields.io/badge/Tool-Power%20BI-yellow)
![Domain](https://img.shields.io/badge/Domain-Data%20Science%20%26%20Analytics-blue)
![Status](https://img.shields.io/badge/Project-Completed-success)
![Internship](https://img.shields.io/badge/Internship-Future%20Interns-purple)

---

## 🚀 Project Overview

This project was completed as Task 3 of my Data Science & Analytics Internship at Future Interns.
The objective of this project is to analyze the marketing funnel performance, identify conversion drop-offs, and evaluate channel-wise effectiveness using an interactive Power BI dashboard.

The dashboard provides a data-driven view of the lead-to-deal journey, helping stakeholders understand:

How leads move through the funnel

Where conversions are lost

Which marketing sources generate the most value

🛠️ Tools & Technologies

Power BI Desktop – Dashboard creation & storytelling

DAX (Data Analysis Expressions) – Conversion & KPI calculations

Microsoft Excel / CSV – Data preparation

Data Modeling – Relationships, measures, and filters

🎯 Business Objectives

This analysis answers critical business questions such as:

How many total marketing leads were generated?

What percentage of leads are converted into deals?

Where are the major funnel drop-offs?

Which marketing channels drive the most leads and won deals?

How do lead types influence deal success?

What is the monthly trend of marketing leads?

Which business types contribute most to won deals?

🖼️ Dashboard Pages Overview
🔹 Page 1: Marketing Funnel & Conversion Overview

Purpose:
Provides a high-level snapshot of the complete marketing funnel and conversion performance.

Key KPIs & Visuals:

Total Marketing Leads

Converted to Deals

Won Deals

Marketing to Deal Conversion (%)

Lead-to-Deal Conversion Funnel

Marketing Leads by Source

Monthly Marketing Leads Trend

🔹 Page 2: Conversion Performance Analysis

Purpose:
Focuses on deep-dive conversion analysis across channels, lead types, and business categories.

Key Visuals:

Won Deals by Marketing Source

Distribution of Won Deals by Business Type

Won Deals by Lead Type (Funnel View)

Deal to Won Conversion %

Marketing to Deal Conversion %

📐 Key DAX Measures Used
Total Marketing Leads = COUNT(marketing_data[lead_id])


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
🔍 Key Insights & Findings

Only ~10.5% of marketing leads successfully convert into won deals, highlighting significant funnel drop-offs.

Organic search and paid search generate the highest number of leads and won deals.

A large drop-off occurs between total leads and converted deals, indicating the need for better lead qualification.

Online medium and online big leads contribute the most to won deals.

Resellers account for the majority of successful deals compared to manufacturers and other business types.

Marketing leads show seasonal fluctuations, with a noticeable dip mid-year.

📌 Conclusion

This marketing funnel analysis clearly highlights where conversions are lost and which channels drive real business value.
By optimizing lead qualification, improving mid-funnel engagement, and focusing on high-performing channels and lead types, organizations can significantly improve their lead-to-customer conversion rates.

The dashboard enables stakeholders to make data-driven marketing and sales decisions with clarity and confidence.

✍️ Author

Omkar Udawant
