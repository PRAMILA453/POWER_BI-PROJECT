💳 Banking Loan Analysis Dashboard (Power BI)
🚀 Overview
This project showcases an interactive Power BI dashboard built using banking datasets — Customers, Accounts, Loans, and Transactions.
The goal is to provide insights into loan distribution, repayment trends, customer profiles, and financial performance for decision-making.

📂 Project Structure
Code
├── data/                # Raw datasets (Customers, Accounts, Loans, Transactions)
├── pbix/                # Power BI project files
├── reports/             # Exported dashboards (PDF/PNG)
└── README.md            # Documentation
🧠 Key Features
Customer Insights: Age, city, and account balance distribution.

Loan Analysis: Loan type distribution, average loan amount, repayment status.

Transaction Insights: Credit vs Debit trends, monthly transaction volume.

KPIs:

Total Loan Amount

Total Balance

Transaction Count

Average Loan Amount

⚙️ Data Preparation
Cleaned loan amounts (removed currency symbols, commas).

Converted dates (JoinDate, TransactionDate, LoanStartDate) into proper Date format.

Built relationships:

Customers.CustomerID → Accounts.CustomerID

Accounts.AccountID → Transactions.AccountID

Customers.CustomerID → Loans.CustomerID

📊 Dashboard Visuals
Insight	Visual Type	Fields
Loan Distribution by Type	Pie Chart	LoanType, LoanAmount
Monthly Transaction Trend	Line Chart	TransactionDate, Amount
Customer Overview	Table	Name, City, Age, Balance, LoanAmount
City-wise Balance	Bar Chart	City, Balance
KPIs	Cards	Total Loan, Total Balance, Transaction Count


🌟 Business Use Cases
Identify top loan types and their contribution to revenue.

Monitor repayment trends and detect risk areas.

Analyze customer demographics for targeted loan offers.

Track transaction behavior to improve banking services.

🛠️ Tech Stack
Tool: Power BI Desktop & Power BI Service

Data Sources: CSV files (Customers, Accounts, Loans, Transactions)

Techniques: Power Query (ETL), DAX Measures, Data Modeling

📌 Future Enhancements
Add Loan Default Prediction using ML integration.

Connect to live SQL database for real-time updates.

Include drill-through reports for customer-level analysis.
