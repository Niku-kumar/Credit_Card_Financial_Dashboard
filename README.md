# 💳 Credit Card Financial Dashboard

A **Power BI Data Analytics project** that analyzes credit card transactions, customer demographics, revenue, interest, income, and spending behavior using **SQL, Power Query, DAX, and Power BI**.

The project transforms raw CSV data into a MySQL database and connects it with Power BI to create interactive dashboards and derive meaningful business insights.

---

## 📊 Dashboard Preview

### 💳 Credit Card Transaction Dashboard

(./Credit Card Financial Dashboard-Transaction.pdf)**

### 👥 Credit Card Customer Dashboard

(./Credit Card Financial Dashboard-Customer.pdf)**

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

Client_Num
Card_Category
Annual_Fees
Activation_30_Days
Customer_Acq_Cost
Week_Start_Date
Week_Num
Qtr
current_year
Credit_Limit
Total_Revolving_Bal
Total_Trans_Amt
Total_Trans_Ct
Avg_Utilization_Ratio
Use_Chip
Exp_Type
Interest_Earned
Delinquent_Acc

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
