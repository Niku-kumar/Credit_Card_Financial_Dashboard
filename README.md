# 💳 Credit Card Financial Dashboard

A **Power BI Data Analytics project** that analyzes credit card transactions, customer demographics, revenue, interest, income, and spending behavior using **SQL, Power Query, DAX, and Power BI**.

The project transforms raw CSV data into a MySQL database and connects it with Power BI to create interactive dashboards and derive meaningful business insights.

---

## 📊 Dashboard Preview

### 💳 Credit Card Transaction Dashboard

📄 [View Transaction Dashboard](./Credit%20Card%20Financial%20Dashboard%20-%20Transaction.pdf)

### 👥 Credit Card Customer Dashboard

📄 [View Customer Dashboard](./Credit%20Card%20Financial%20Dashboard%20-%20Customer.pdf)

---

## 🚀 Project Overview

The objective of this project is to analyze **credit card financial and customer data** and create an interactive Business Intelligence dashboard.

The dashboard provides insights into:

- 💰 Revenue and interest earned
- 💳 Credit card transaction amounts and counts
- 📈 Weekly and quarterly revenue trends
- 👥 Customer demographics
- 💼 Customer job categories
- 🎓 Education levels
- 💵 Income groups
- 💳 Card categories
- 🛒 Expenditure types
- 📍 State-wise customer distribution
- 🔄 Chip, swipe, and online transaction usage
- 🎯 Customer acquisition cost

---

## 🛠️ Tools & Technologies

| Technology | Purpose |
|---|---|
| **MySQL** | Database creation and data storage |
| **SQL** | Data processing and querying |
| **Power Query** | Data cleaning and transformation |
| **DAX** | Measures and calculations |
| **Power BI** | Data visualization and dashboard creation |
| **CSV** | Raw data source |

---

## 🔄 Project Workflow

```text
CSV Files
    ↓
MySQL Database
    ↓
SQL Data Processing
    ↓
Power BI Connection
    ↓
Power Query
    ↓
Data Modeling
    ↓
DAX Measures
    ↓
Interactive Dashboard
    ↓
Business Insights

---

🗄️ Database Structure

The project uses two main tables.

1. cc_detail

Contains credit card transaction and financial information.

Important columns include:

• Client_Num
• Card_Category
• Annual_Fees
• Activation_30_Days
• Customer_Acq_Cost
• Week_Start_Date
• Week_Num
• Qtr
• current_year
• Credit_Limit
• Total_Revolving_Bal
• Total_Trans_Amt
• Total_Trans_Ct
• Avg_Utilization_Ratio
• Use_Chip
• Exp_Type
• Interest_Earned
• Delinquent_Acc

2. cust_detail

Contains customer demographic and financial information.

Important columns include:

• Client_Num
• Customer_Age
• Gender
• Dependent_Count
• Education_Level
• Marital_Status
• State_cd
• Zipcode
• Car_Owner
• House_Owner
• Personal_Loan
• Contact
• Customer_Job
• Income
• Cust_Satisfaction_Score
• 🧹 Data Processing

The raw CSV files were first imported into MySQL.

Additional weekly data was also loaded into the database before connecting the database with Power BI.

---

Database Creation
CREATE DATABASE ccdb;
Credit Card Details Table
CREATE TABLE cc_detail (
    Client_Num INT,
    Card_Category VARCHAR(20),
    Annual_Fees INT,
    Activation_30_Days INT,
    Customer_Acq_Cost INT,
    Week_Start_Date DATE,
    Week_Num VARCHAR(20),
    Qtr VARCHAR(10),
    current_year INT,
    Credit_Limit DECIMAL(10,2),
    Total_Revolving_Bal INT,
    Total_Trans_Amt INT,
    Total_Trans_Ct INT,
    Avg_Utilization_Ratio DECIMAL(10,3),
    Use_Chip VARCHAR(10),
    Exp_Type VARCHAR(50),
    Interest_Earned DECIMAL(10,3),
    Delinquent_Acc VARCHAR(5)
);
Customer Details Table
CREATE TABLE cust_detail (
    Client_Num INT,
    Customer_Age INT,
    Gender VARCHAR(5),
    Dependent_Count INT,
    Education_Level VARCHAR(50),
    Marital_Status VARCHAR(20),
    State_cd VARCHAR(50),
    Zipcode VARCHAR(20),
    Car_Owner VARCHAR(5),
    House_Owner VARCHAR(5),
    Personal_Loan VARCHAR(5),
    Contact VARCHAR(50),
    Customer_Job VARCHAR(50),
    Income INT,
    Cust_Satisfaction_Score INT
);

CSV data was imported into MySQL using LOAD DATA LOCAL INFILE.

---

📈 Power BI Dashboard

The dashboard contains multiple visualizations, KPI cards, filters, and interactive charts.

• Key KPIs
• Total Revenue: 57M
• Total Interest: 8M
• Income: 588M
• Total Transactions: 667K
• Transaction Amount: 46M
• Customer Satisfaction Score: 3.19

KPI values are based on the dashboard analysis.

---

📊 Dashboard Analysis

Credit Card Transaction Report

The dashboard analyzes:
• Revenue by quarter
• Total transaction count
• Revenue by card category
• Revenue by expenditure type
• Revenue by education
• Revenue by customer job
• Revenue by chip usage
• Customer acquisition cost

Credit Card Customer Report

The dashboard provides:
• Revenue by week
• Revenue by age group
• Revenue by customer job
• Top 5 states
• Revenue by marital status
• Revenue by income group
• Revenue by dependents
• Revenue by education
• Gender-based analysis

---

🔍 Key Insights

• The dashboard helped identify several important business insights:
• Swipe transactions contribute the highest revenue compared with chip and online transactions.
• Blue card customers contribute the largest share of revenue among card categories.
• Graduate customers generate significant revenue compared with other education groups.
• Businessman customers are among the highest revenue-generating customer segments.
• Revenue varies significantly across different income groups, age groups, states, and customer jobs.
• Quarterly analysis helps identify changes in revenue and transaction volume.
• Customer acquisition cost differs across different card categories.

---

📚 Topics Covered
• Connecting Power BI with SQL Database
• Importing data into Power BI
• Importing CSV data into MySQL
• SQL database and table creation
• SQL data processing
• Power Query
• Data cleaning and transformation
• DAX
• DAX measures
• Charts and tables
• KPI cards
• Slicers and filters
• Dashboard design
• Business Intelligence
• Data visualization
• Business insights

---

🎯 Learning Outcomes

This project helped me strengthen my practical understanding of:

SQL → Data Processing → Power Query → DAX → Power BI → Business Insights

It provided hands-on experience in transforming raw data into an interactive, business-focused dashboard and extracting meaningful insights from customer and transaction data.

---

👨‍💻 Author

Niku Kumar Yadav

B.Tech CSE Student | Data Analytics & Power BI Enthusiast
