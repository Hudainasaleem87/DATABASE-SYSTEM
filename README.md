# DATABASE-SYSTEM
this project is part of our Artificial Intelligence Semester course DBMS
# Retail Store Database (retail_store_db)

This project contains the design and implementation of a relational database for managing a retail store. It was created as part of my semester course to demonstrate database design, SQL queries, normalization, and real-world data management.

---

## 📌 Project Overview

The **retail_store_db** database manages information related to:

- Customers  
- Products  
- Categories  
- Orders  
- Order Items  
- Inventory  
- Suppliers  
- Payments
- Users  

The database is normalized (up to 3NF) to reduce redundancy and maintain data integrity.

---

## 🏗️ Database Structure

### Main Tables
- **customers**
- **products**
- **categories**
- **orders**
- **order_items**
- **inventory**
- **suppliers**
- **payments**
- **Users**

### Key Features
- Proper primary and foreign key relationships  
- Constraints for integrity  
- Sample data for testing  
- Useful analytical queries  

---

## 🛠️ Technologies Used
- MySQL (or MariaDB)  
- SQL (DDL & DML)  
- Optional: MySQL Workbench / XAMPP / phpMyAdmin  

---

## 🚀 How to Run the Project

### 1. Install MySQL
Make sure MySQL Server or XAMPP/WAMP/MAMP is installed.

### 2. Create the Database
Run the following:

```sql
CREATE DATABASE retail_store_db;
USE retail_store_db;
```

### 3. Import the SQL File
If you have `retail_store_db.sql`, import it:

#### Using MySQL Workbench
1. Open Workbench  
2. File → Open SQL Script  
3. Select the SQL file  
4. Execute

#### Using Command Line
```bash
mysql -u root -p retail_store_db < retail_store_db.sql
```

#### Using phpMyAdmin
1. Open phpMyAdmin  
2. Select/Create `retail_store_db`  
3. Go to **Import**  
4. Upload the SQL file  
5. Click **Go**

---

## ▶️ Running Queries

You can now run queries such as:

```sql
SELECT c.customer_name, o.order_date, p.product_name
FROM customers c
JOIN orders o ON c.customer_id = o.customer_id
JOIN order_items oi ON o.order_id = oi.order_id
JOIN products p ON oi.product_id = p.product_id;
```

---

## 🎯 Purpose of This Project
This database project was developed as part of my semester coursework to practice:

- Database design  
- Entity-Relationship modeling  
- SQL implementation  
- Query optimization  
- Relational schema development  

---

## 📬 Notes
If submitting for class, include:

**Maryam Abdulah AND Hudaina Muhammad Saleem:**  
**Database System**  
**4th Semester**  
**Mister Anwar Ali Sathio**  


