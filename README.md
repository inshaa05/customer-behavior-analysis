# customer-behavior-analysis
End-to-end Data Analytics project analyzing customer purchasing behavior using Python, PostgreSQL, SQL, and Power BI.
# 📊 Customer Behavior Data Analysis

The project covers the complete analytics workflow — from data cleaning and preparation to SQL analysis and interactive dashboard development — with the goal of identifying patterns in customer behavior, purchasing trends, and subscription activity.

## 📌 Project Overview

This project analyzes customer transaction data to answer business-focused questions such as:

* Which products and categories generate the most revenue?
* How do purchasing patterns vary across customer demographics?
* Are repeat customers more likely to subscribe?
* Which products are most frequently purchased?
* How does revenue vary across different age groups?
* What patterns can be identified from customer purchasing behavior?

The analysis combines **Python for data preparation, PostgreSQL for querying and analysis, and Power BI for interactive visualization**.


## 🛠️ Tools & Technologies

| Tool               | Purpose                                      |
| ------------------ | -------------------------------------------- |
| 🐍 **Python**      | Data cleaning and preparation                |
| 🐼 **Pandas**      | Data manipulation and transformation         |
| 🗄️ **PostgreSQL** | Data storage and SQL analysis                |
| 🔎 **SQL**         | Business-focused data analysis               |
| 📊 **Power BI**    | Data visualization and dashboard development |
| 📗 **Excel**       | Data transfer and Power BI integration       |


## 🔄 Project Workflow

Raw Customer Data
       ↓
Python / Pandas
       ↓
Data Cleaning & Preparation
       ↓
PostgreSQL
       ↓
SQL Analysis
       ↓
Power BI
       ↓
Interactive Dashboard
       ↓
Business Insights

## 🐍 1. Data Preparation with Python

Python and Pandas were used to prepare the customer dataset before analysis.

Key steps included:

* Loading the raw dataset
* Inspecting data structure and data types
* Identifying missing values
* Checking for duplicate records
* Cleaning and standardizing data
* Preparing the dataset for database analysis
* Exporting the cleaned dataset for downstream analysis

## 🗄️ 2. PostgreSQL & SQL Analysis

The cleaned dataset was loaded into PostgreSQL, where SQL was used to answer business questions and identify customer behavior patterns.

Examples of analysis include:

### 🔹 Top Products by Category

Used SQL window functions such as `ROW_NUMBER()` to identify the top products within each category.

### 🔹 Repeat Customer Analysis

Customers with more than five previous purchases were analyzed by subscription status.

```sql
SELECT subscription_status,
       COUNT(customer_id) AS repeat_buyers
FROM customer
WHERE previous_purchases > 5
GROUP BY subscription_status;
```

### 🔹 Revenue by Age Group

Customer revenue was analyzed across different age groups to understand which segments contribute most to overall sales.

Other SQL analysis included:

* Product purchasing frequency
* Category-level performance
* Customer segmentation
* Subscription behavior
* Revenue analysis
* Purchasing patterns


## 📊 3. Power BI Dashboard

The cleaned and analyzed data was brought into Power BI to create an interactive dashboard.

The dashboard provides an overview of:

* 💰 Revenue & sales performance
* 👥 Customer demographics
* 🛍️ Product & category performance
* 🔄 Customer purchasing behavior
* ⭐ Review ratings
* 📦 Shipping and purchasing patterns
* 🔔 Subscription status

### Dashboard Preview

<img width="1188" height="639" alt="image" src="https://github.com/user-attachments/assets/b07372f7-f635-408a-bf16-d64b204e649f" />


## 💡 Key Insights

The analysis was used to identify patterns in:

* Customer purchasing behavior
* Repeat purchasing activity
* Subscription adoption
* Revenue contribution across customer segments
* Product and category performance
* Demographic purchasing patterns

These insights demonstrate how raw customer data can be transformed into **actionable business information through SQL analysis and BI dashboards**.

## 🎯 Skills Demonstrated

* Data Cleaning
* Exploratory Data Analysis
* Python & Pandas
* PostgreSQL
* SQL Querying
* Data Aggregation
* Window Functions
* Customer Segmentation
* Business Analysis
* Power BI
* Data Visualization
* Dashboard Development
* End-to-End Data Analytics
