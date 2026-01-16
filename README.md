# Task 2: Data Types, Constraints & Table Design

## 📌 Task Overview
This task focuses on designing a proper SQL table schema using correct data types and constraints. It helps in understanding how databases enforce data integrity and how table structures can be modified safely using SQL commands.

---

## 🛠 Tools Used
- **Primary:** MySQL Workbench  
- **Alternatives:** PostgreSQL, SQLite, DBeaver  

---

## 📂 Project Files
- `task2_table_design.sql` → SQL script with table creation, constraints, and alterations  
- `README.md` → Task documentation  

---

## 🎯 Objectives
- Redesign an existing table using appropriate SQL data types
- Apply constraints to ensure data integrity
- Understand the importance of validation rules
- Practice modifying table structure using `ALTER TABLE`
- Observe constraint failures by inserting invalid data

---

## 🗄 Database & Table Details
- **Database Name:** `intern_training_db`
- **Table Name:** `students`

### Table Structure:
| Column Name | Data Type | Constraints | Description |
|-----------|----------|------------|-------------|
| student_id | INT | PRIMARY KEY, AUTO_INCREMENT | Unique student identifier |
| full_name | VARCHAR(60) | NOT NULL | Student full name |
| email | VARCHAR(100) | UNIQUE, NOT NULL | Student email address |
| date_of_birth | DATE | NOT NULL | Date of birth |
| age | INT | CHECK (age >= 0) | Student age |
| created_at | TIMESTAMP | DEFAULT | Record creation time |

---

## 🔐 Constraints Used & Purpose
- **PRIMARY KEY:** Ensures each record is unique
- **NOT NULL:** Prevents missing critical data
- **UNIQUE:** Avoids duplicate email entries
- **CHECK:** Validates allowed values
- **DEFAULT:** Automatically assigns values

Constraints help maintain **data accuracy, consistency, and reliability**.

---

## 🔧 SQL Operations Performed
1. Dropped and recreated table with improved design
2. Inserted valid records
3. Tested constraint violations using invalid data
4. Added a new column using `ALTER TABLE`
5. Renamed an existing column
6. Dropped a column and understood its impact
7. Verified table structure and data

---

## ▶ How to Run
1. Open **MySQL Workbench**
2. Select database `intern_training_db`
3. Open `task2_table_design.sql`
4. Execute queries step by step
5. Observe results and error messages for invalid inputs

---

## ✅ Final Outcome
By completing this task, the intern:
- Understands SQL data types and constraints
- Learns why constraints are critical for data integrity
- Gains experience modifying schemas safely
- Builds strong foundational skills in database design

---

## 📌 Author
**Intern Name:** _(Your Name)_  
**Task:** SQL Internship – Task 2  
**Status:** Completed ✅
