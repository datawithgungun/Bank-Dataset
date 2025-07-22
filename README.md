# Bank-Dataset-by-using-SQL

# 🏦 Bank Database Analysis using SQL

This project demonstrates how to analyze structured banking data stored in a relational database using SQL queries. It includes insights into customer profiles, account details, transaction trends, loan distributions, and branch/ATM statistics.

## 📁 Database Tables Used

The database schema consists of the following main tables:

| Table Name          | Description                                  |
| ------------------- | -------------------------------------------- |
| `customers_data`    | Customer details (ID, name, contact info)    |
| `accounts_data`     | Account info (account number, type, balance) |
| `transactions_data` | Records of customer transactions             |
| `loans_data`        | Loan info (amount, status, type)             |
| `branches_data`     | Branch locations and details                 |
| `atms_data`         | ATM details by location and usage            |

## 🎯 Project Objectives

* Write SQL queries to:

  * Analyze customer demographics and account ownership
  * Track transaction patterns and frequency
  * Study branch and ATM activity
  * Analyze loan distribution and repayment status
* Create views and stored procedures for recurring reports
* Use joins, aggregations, subqueries, and window functions for deep insights

## 🛠️ Tools & Technologies

* **MySQL / PostgreSQL** (or any RDBMS)
* **SQL Workbench / DBeaver / pgAdmin** for query execution
* **Power BI / Excel** (optional - for visualization)

## 🔍 Sample SQL Tasks

Here are examples of the types of queries included:

```sql
-- 1. Total number of customers
SELECT COUNT(*) FROM customers_data;

-- 2. Top 5 branches by total loan amount
SELECT branch_id, SUM(loan_amount) AS total_loans
FROM loans_data
GROUP BY branch_id
ORDER BY total_loans DESC
LIMIT 5;

-- 3. Monthly transaction summary
SELECT MONTH(transaction_date) AS month, COUNT(*) AS transaction_count
FROM transactions_data
GROUP BY MONTH(transaction_date);
```

## 📊 Analysis Highlights

* Top performing branches in terms of customer base and loan disbursement
* Customer behavior based on transaction volume and frequency
* ATM distribution and usage patterns by location
* Ratio of active to inactive accounts

## 🧠 Future Enhancements

* Create indexes for performance tuning
* Integrate SQL views for reusable insights
* Add stored procedures for monthly reports
* Connect database to Power BI for live dashboards

## 📌 Author

**Gungun Anant Chavan**
📍 Nagpur, Maharashtra
📧 [chavangungun657@gmail.com](mailto:chavangungun657@gmail.com)
🔗 [LinkedIn](https://www.linkedin.com/in/gungun-chavan-822440259/) | [GitHub](https://github.com/datawithgungun)

---
