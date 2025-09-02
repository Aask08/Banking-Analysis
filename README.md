📊 Banking Risk Analytics & Dashboard
📌 Project Overview

This project demonstrates risk analytics in banking and financial services using data-driven techniques. The primary goal is to analyze banking data and build interactive Power BI dashboards that help financial institutions minimize risk while lending money to customers.

By leveraging ETL (Extract, Transform, Load), KPIs, calculated measures, and visualization, the dashboards support decision-making on whether an applicant is likely to repay a loan.

🏦 Problem Statement

Banks face the challenge of identifying reliable clients while minimizing lending risks. The task is to develop a data-driven approach to:

Understand customer profiles

Evaluate risk associated with loans

Track deposits, loans, and fees

Improve decision-making in financial operations

🛠️ ETL Workflow (Jupyter Notebook)

The ETL pipeline was implemented in the Jupyter notebook to prepare data before visualization in Power BI:

🔹 Extract

Loaded raw banking datasets (multiple CSV/Excel files containing Client-Banking, Banking Relationship, Gender, Advisor, Period).

Connected data using pandas for initial exploration.

🔹 Transform

Cleaned missing values and removed duplicates.

Created new columns:

Engagement Timeframe → client’s duration with the bank

Engagement Days → number of days since joining

Income Band → categorized income as Low (<100k) and Mid (<300k)

Processing Fees → computed fee = 0.05 * Loan for high fee structure clients

Converted categorical variables into standardized formats for analysis.

Aggregated measures (loans, deposits, fees) using groupby and DAX-style transformations.

🔹 Load

Final cleaned dataset exported as .csv and integrated with Power BI for dashboard creation.

Structured tables were linked in Power BI using primary/foreign keys for relational modeling.

🗂️ Dataset

The dataset contains multiple interconnected tables linked with primary and foreign keys:

Banking Relationship

Client-Banking

Gender

Investment Advisor

Period

⚙️ Calculated Functions & DAX

Some of the key DAX functions used include:

SUM() → Aggregation of deposits, loans, and accounts

DISTINCTCOUNT() → Unique client counts

SUMX() → Row-wise calculations for fees & loans

DATEDIFF() → Engagement duration in days

SWITCH() → Custom categorical calculations

📈 Key Performance Indicators (KPIs)

The dashboards track essential banking KPIs such as:

Total Clients → 188

Total Loan → $139.9M

Total Deposit → $111.49M

Total Fees → $5.17M

Total Engagement Account → $18.26K

Total Credit Card Account → $135

📊 Dashboards & Visualizations

Developed in Power BI:

Home Dashboard – Overview of clients and banking metrics

Loan Analysis – Loan distribution by income band, nationality, and client type

Deposit Analysis – Deposits across various accounts (savings, checking, foreign currency)

Summary Dashboard – Consolidated view of KPIs and insights

✅ Results & Insights

Identified which banks have the highest number of clients (private banks lead).

Insights on loan distribution by nationality and income band.

Tracking of account types: savings, checking, deposits, foreign currency, and credit card balances.

Support for financial goal planning and client engagement tracking.

🔮 Future Work

Expand analysis to include default prediction models.

Integrate real-time data for live dashboards.

Extend insights to cross-sell opportunities (credit cards, investments).

Benchmark performance across different banking institutions.

📂 Project Files

BankEDA (Version 2).ipynb → ETL + EDA Notebook

Banking Report.docx → Detailed Project Report

Banking.pptx → Project Presentation

👥 Contributors

Mohammad Aas Khan
