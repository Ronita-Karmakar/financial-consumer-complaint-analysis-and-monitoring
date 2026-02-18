# financial-consumer-complaint-analysis-and-monitoring

# Project Overview
This project focuses on analyzing consumer complaints related to financial products and services received by Bank of America through the Consumer Financial Protection Bureau (CFPB). The goal was to build a centralized tracking and monitoring system to analyze complaint trends, response timelines, and compliance performance.

The solution provides insights into complaint volume, delay patterns, response effectiveness, and operational risks using interactive data visualization.

# Business Problem
The Compliance Department at Bank of America receives consumer complaints from the Consumer Financial Protection Bureau (CFPB) related to financial products and services. However, there is no centralized tracking mechanism to effectively monitor open and closed complaints, response timelines, and weekly trends.

Without proper tracking and trend analysis, complaints may become overdue, leading to compliance risks, delayed resolutions, and potential regulatory penalties.

Therefore, there is a need to develop a structured Consumer Complaint Tracking Report to monitor complaint status, analyze weekly trends, and ensure timely handling and regulatory compliance.

# Tech Stack
- Excel (Data Source)
- Python (Pandas, NumPy)
- MySQL
- Power BI

# Solution Approach

The project follows an end-to-end data analytics workflow:

1️⃣ **Data Cleaning & Preprocessing (Python)**
- Cleaned raw complaint dataset
- Standardized column naming and formatting
- Handled missing values and data types
- Created derived fields:
    - Processing days
    - Complaint week
    - Timely response flag
    - Overdue flag
    - Complaint year and month

2️⃣ **Data Storage (MySQL)**
- Designed structured database schema
- Created tables for cleaned data
- Loaded processed dataset into MySQL for centralized storage

3️⃣ **Power BI Dashboard**
<img width="1050" height="685" alt="image" src="https://github.com/user-attachments/assets/e5c69ddc-6c22-41b3-91c7-f52dd1c11e22" />
<img width="1200" height="575" alt="image" src="https://github.com/user-attachments/assets/87f0ec56-2368-4fbb-828e-84fe4ead9868" />

Power BI is connected directly to the MySQL database to build interactive dashboards.

Two dashboard pages were created:

**Key Insights — Overview Dashboard**

**Complaint Volume Trends**
- Complaint volume peaks during July–August.
- Delay counts increase during high workload periods.

**Weekly Trend Analysis**
- Sudden spikes correlate with increased delays.
- Indicates need for operational scaling during peak weeks.

**Product Analysis**
- Checking accounts generate the highest complaint volume (~25K).
- Credit cards and credit reporting also significant.

**Response Timeliness**
- Majority handled within SLA timelines.
- High-volume issue categories still drive delays.

**Delay Rate by Issue**
- Overdraft/savings issues show higher delay risk.

<br>

**Key Insights — Delay & Operational Analysis**

**Highest Delay Category**
Monetary relief cases show highest delay rate.

**Submission Channel Analysis**
- Web channel dominates (~45K complaints).

**Channel Performance**
- High timely response rates across channels.

**Processing Time by Issue**
- Excessive fees require longest resolution time.
- Advertising issues resolve faster.

**Regional Analysis**
- California shows highest complaint volume.

**Resolution Outcome Analysis**
- Monetary relief cases correlate with higher delays.

# Recommendations
- Improve workflow automation for monetary relief cases.
- Optimize web submission workflows and validation.
- Standardize investigation processes for complex issues.
- Strengthen regional resource allocation.
- Implement early delay detection alerts for SLA monitoring.

# Conclusion
This project demonstrates an end-to-end financial consumer complaint analysis workflow, transforming raw data into actionable insights using Python, MySQL, and Power BI. 
By tracking complaint trends, response timelines, and delay risks, the solution supports compliance monitoring and data-driven decision-making, helping identify operational inefficiencies, high-risk categories, and opportunities to improve response efficiency and customer service outcomes.
