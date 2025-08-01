# JDBC Employee Manager

A simple Java application that demonstrates how to connect to a MySQL database using JDBC, insert employee records, and retrieve them.

---

## 📌 Project Overview

This project is intended for beginners to understand the basics of JDBC operations including:

- Connecting to a MySQL database
- Executing parameterized SQL queries
- Reading data using `ResultSet`
- Safe resource management using try-with-resources

---

## 🗂️ File Structure

JDBC-Employee-Manager/
├── Main1.java # Java code that performs DB operations
├── mec.sql # SQL script to create database and table
└── README.md # Project documentation


---

## 🚀 Features

- ✅ Connects to local MySQL using JDBC
- ✅ Inserts employee data using `PreparedStatement`
- ✅ Retrieves and prints all employees from the database
- ✅ Automatically closes database resources
- ✅ Well-suited for Java and database learning

---

## 🛠️ Prerequisites

To run this project, you need:

- Java JDK 8 or higher
- MySQL Server installed
- MySQL JDBC Driver (e.g., `mysql-connector-java-8.x.x.jar`)
- Basic terminal or IDE setup

---

## 🧩 Setup Instructions

### 1. 🧱 Database Setup

1. Open MySQL command line or MySQL Workbench.
2. Run the following SQL script or use `mec.sql`:

```sql
-- Create database and table
CREATE DATABASE IF NOT EXISTS mec;

USE mec;

CREATE TABLE IF NOT EXISTS employees (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100),
    salary DOUBLE
);


💻 Sample Output

--- Executing INSERT ---
1 row(s) inserted successfully
1 row(s) inserted successfully
----EXECUTING SELECT----
Employee Data
-----------------------
ID: 1, Name: JOHAN DOE, Salary: 50000.00
ID: 2, Name: Jane Smith, Salary: 65000.00
