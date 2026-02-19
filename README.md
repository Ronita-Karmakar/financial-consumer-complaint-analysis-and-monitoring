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

**Key Metrics:**
- 62,520 Total Complaints
- 93.77% Timely Response Rate
- 6.23% Delay Rate
- 1.22 Days Average Processing Time

**Complaint Volume Trends**

- Checking/Savings & Credit Cards generate highest complaints
- Complaint spike observed during July–August
- Specific issue categories show higher delay rates
- Weekly trend monitoring helps detect operational backlog
- Overdraft/savings issues show higher delay risk.

<br>

**Key Insights — Delay & Operational Analysis**

- Fee-related complaints take longest to resolve (~5 days)
- Monetary relief cases have higher delay percentage
- Web channel dominates complaint submissions
- California has highest complaint concentration
- Operational complexity increases delay probability

# Recommendations
- Improve workflow automation for monetary relief cases.
- Optimize web submission workflows and validation.
- Standardize investigation processes for complex issues.
- Strengthen regional resource allocation.
- Implement early delay detection alerts for SLA monitoring.

# Conclusion
This project demonstrates an end-to-end financial consumer complaint analysis workflow, transforming raw data into actionable insights using Python, MySQL, and Power BI. 
By tracking complaint trends, response timelines, and delay risks, the solution supports compliance monitoring and data-driven decision-making, helping identify operational inefficiencies, high-risk categories, and opportunities to improve response efficiency and customer service outcomes.
