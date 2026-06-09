# 🧹 SQL Exercise — NULL Functions

## 📌 Overview
This repository contains a **handwritten SQL exercise** focused on handling NULL values.

The exercise is part of my SQL learning journey and was completed manually to strengthen my understanding of how to work with incomplete data.

---

## ✍️ Exercise Approach

For this exercise, I:

- Wrote all SQL queries by hand  
- Practiced problem-solving without using a SQL tool  
- Focused on understanding how NULL values affect data  
- Drew expected output tables for each question  

📎 The handwritten solutions are scanned and included in this repository.

---

## 🎯 Concepts Covered

The exercise covers key NULL handling techniques used in SQL:

- `COALESCE()`  
- `IFNULL()` / `ISNULL()`  
- `CASE WHEN`  
- `COUNT()` with NULL filtering  

---

## 🧠 What I Practiced

- Replacing NULL values with defaults  
- Handling missing text and numeric data  
- Writing clean and readable SQL logic  
- Understanding how NULL impacts analysis  

---

## 📊 Example

Handling missing salary values:

```sql
SELECT 
    employee_id,
    name,
    IFNULL(salary, 0) AS salary_with_default
FROM employees;
```

---

## 📂 Repository Contents

- 📄 Handwritten SQL solutions (scanned)
- 📊 Exercise questions
- ✅ Expected outputs (drawn tables)

---

## 🚀 Learning Outcome

This exercise helped me:
- Build strong SQL fundamentals
- Improve logical thinking
- Understand real-world data cleaning scenarios
- Gain confidence in writing SQL without tools
