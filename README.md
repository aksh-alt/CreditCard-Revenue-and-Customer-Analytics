# CreditCard-Revenue-and-Customer-Analytics
End-to-end financial analytics solution in Power BI using SQL, DAX, and weekly data updates for credit card transaction and customer insights.
![Screenshot 2025-05-30 214827](https://github.com/user-attachments/assets/38a8b4a5-90c9-49fa-afc7-561b279dc3e8)



 💳 **Credit Card Transaction & Customer Insights Dashboard**

### 📌 Introduction

This dual-dashboard Power BI project provides a detailed overview of credit card transactions and customer behavior, offering actionable insights for financial institutions. The reports combine SQL-based data modeling, dynamic DAX calculations, and interactive visual storytelling to monitor key KPIs such as revenue, transaction trends, interest earnings, and customer satisfaction.

The analysis helps understand customer segments, usage preferences, revenue drivers, and behavioral patterns, crucial for targeted marketing and product optimization in the financial sector.

---

### 🛠 Tools & Skills Used

- 🧮 **SQL (PostgreSQL)** – Created database and tables, imported CSVs
- 🔗 **Power BI** – Dashboards & Visualizations
- 🔧 **Power Query** – Data cleaning & transformation
- 💡 **DAX** – Advanced measures for current & previous week calculations, bucketing, KPI logic
- 📅 **Time Intelligence** – Used `WEEKNUM`, `MAX`, `FILTER`, `ALL`, `SWITCH`, etc.
- 🧠 **Data Modeling** – Connected weekly updates to existing tables for seamless refresh
---
![Screenshot 2025-05-31 130422](https://github.com/user-attachments/assets/130ec998-058d-4fd6-8f8c-758a13f68dbb)




![Screenshot 2025-05-31 130458](https://github.com/user-attachments/assets/eedbcf14-1df3-4332-91f4-033687fb4bb0)





### 🗃️ Dataset Details

- **Source:** CSVs from  Kaggle
- **Database:** Created a PostgreSQL database named `CreditCardDB`
- **Tables Created:**
  - `creditcard_transaction` – 18 columns, 10,109 rows
  - `credit_card_customers` – 15 columns, 10,109 rows
- **Additional Weekly Data:** Integrated seamlessly to update visuals with each refresh

---

## 📊 Dashboard Build

### 1️⃣ Credit Card Transaction Report

- 🔍 **Slicers:** Month, Quarter, Card Type, Income Group, Gender
- 📈 **KPIs:** Revenue (55M), Transaction Amount (45M), Interest (8M), Transaction Count (656K)
- 📊 **Visuals:**
  - Table: Revenue, Total Transactions, Interest by Card Category
  - Bar Charts: Revenue by Card Category, Education Level, Customer Job, Expenditure Type
  - Line + Column Chart: Quarterly Revenue vs Transaction Count
  - Revenue by Chip Usage (Swipe, Chip, Online)

---
![Screenshot 2025-05-30 215139](https://github.com/user-attachments/assets/69bf0282-e7ef-42ac-ae15-19a0576d2e80)

### 2️⃣ Credit Card Customer Report

- 🔍 **Slicers:** Month, Quarter, Card Type, Chip Usage, Gender
- 📈 **KPIs:** Revenue (55M), Income (576M), Interest (8M), CSS (3.2)
- 📊 **Visuals:**
  - Age Group & Dependents Analysis
  - Top 5 States by Revenue
  - Education Level Breakdown
  - Weekly Revenue Trends (Line Chart) – Split by Gender
  - Marital Status vs Revenue
  - Income Group Analysis
  - Summary Table: Customer Job vs Revenue, Interest Earned, Income
  - **Legend-Based Coloring:** Red = Male, Orange = Female (Gender-based analysis)

---

### ⚙️ Advanced Techniques Used

- **Nested DAX Measures:** For calculating current and previous week revenue
- **Revenue Calculation Logic:** Revenue = Interest + Annual Fee + Transaction Amount
- **SWITCH Function:** Used for bucketing age & income
- **SQL Table Linking:** Used PostgreSQL to manage data structure before importing to Power BI
- **Incremental Data Refresh:** Appended new week’s data and refreshed visuals without dashboard rebuild

---

## 💡 Key Insights

- 🔵 **Blue category cards** generated the highest revenue (46M)
- 🎓 **Graduate customers** contributed the most to revenue (22M)
- 🧾 **Bills & Entertainment** were top expense categories
- 🖐 **Swipe method** was the most preferred card usage type (35M)
- 🔴 **Male customers** in high-income groups drove most of the revenue
- 📉 Lowest revenue was generated by **female customers** during week 21

---

## 🧾 Conclusion

This project demonstrates a complete financial reporting workflow — from SQL database creation and multi-source integration to complex DAX logic and dashboard storytelling. It is valuable for:

- 📊 **Credit analysts** to segment customer profitability
- 🏦 **Financial teams** to monitor KPIs like revenue and transaction growth
- 💡 **Marketing teams** to identify target segments by age, income, and card usage
- 🔄 **Product teams** to evaluate card types and customer experience for better strategy

With dynamic filtering, real-time refresh, and gender-based insights, this project reflects a high-impact business intelligence solution in the financial analytics space.

---
