# 🧹 Advanced SQL Project — NULL Handling & Data Cleaning

## 📌 Overview
This project demonstrates advanced SQL techniques for handling NULL values across multiple real-world datasets.

Missing data is one of the most common challenges in data analytics, and this project shows how to clean, transform, and prepare data for analysis using SQL.

---

## 🎯 Objective

- Handle missing (NULL) values effectively  
- Replace NULLs with meaningful defaults  
- Build clean, analysis-ready datasets  
- Apply SQL logic used in real business environments  

---

## 📊 Dataset Description

This project includes 16 structured tables, each simulating a real business scenario:

- Employees (missing salaries & departments)  
- Orders (missing customer and delivery info)  
- Students (missing grades)  
- Products (missing discounts)  
- Customers (missing emails)  
- Payments (missing methods/status)  
- Inventory (missing quantities)  
- Bank accounts, projects, reviews, suppliers, and more  

---

## 🧠 Key SQL Skills Demonstrated

### ✅ Replace NULL Values
```sql
SELECT 
    employee_id,
    name,
    COALESCE(salary, 0) AS salary_with_default
FROM employees;
```
### ✅ Replace NULL Text Values
```SQL
SELECT   employee_id,    
            name,    
            COALESCE(department, 'Not Assigned') AS department_name
FROM employees;
```

### ✅ Count Missing Values
```SQL
SELECT COUNT(*) AS missing_email_count
FROM customersWHERE email IS NULL;
```

### ✅ First Non-NULL Value (COALESCE)
```SQL
SELECT  emp_id,    
        COALESCE(bonus, commission) AS first_available_reward
FROM employees_extra;
```

### ✅ Multiple Default Values
```SQL
SELECT  user_id,    
        IFNULL(theme, 'Light') AS theme_set,    
        IFNULL(language, 'English') AS language_set,    
        IFNULL(timezone, 'UTC') AS timezone_set
FROM user_settings;
```

## 🧪 Example Problem
Scenario: Replace missing salary and department values
```SQL
SELECT  employee_id,    
        name,    
        IFNULL(department, 'Not Assigned') AS department_name,    
        IFNULL(salary, 0) AS salary_with_default
FROM employees;
```

---
## 📈 Business Value
This project demonstrates how SQL is used to:

Clean messy datasets
Prepare data for dashboards and reporting
Handle incomplete information in real systems
Improve data quality and consistency

---
## 🛠️ Tools Used

SQL (ANSI SQL / Databricks SQL)
GitHub
CSV datasets

---
## 🚀 Key Takeaways

NULL values must always be handled before analysis
COALESCE is one of the most powerful SQL functions
Clean data = reliable insights
Data preparation is a critical part of analytics workflows
