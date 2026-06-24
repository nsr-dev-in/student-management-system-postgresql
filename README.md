# 🎓 Student Management System using PostgreSQL

A beginner-friendly SQL project built using PostgreSQL to manage student records and perform data retrieval, filtering, sorting, and database operations.

---

## 📌 Project Overview

This project simulates a Student Management System used by colleges to store and manage student information.

The project demonstrates:

- Database Creation
- Table Creation
- Data Insertion
- Data Retrieval
- Data Filtering
- Data Sorting
- CRUD Operations
- NULL Handling

---

## 🛠 Technologies Used

- PostgreSQL
- SQL

---

## 📂 Database Schema

### Students Table

| Column | Data Type |
|----------|------------|
| student_id | SERIAL PRIMARY KEY |
| name | VARCHAR(100) |
| age | INT |
| course | VARCHAR(50) |
| city | VARCHAR(50) |
| email | VARCHAR(100) |
| marks | INT |

---

## 🏗 Create Table

```sql
CREATE TABLE students (
    student_id SERIAL PRIMARY KEY,
    name VARCHAR(100),
    age INT,
    course VARCHAR(50),
    city VARCHAR(50),
    email VARCHAR(100),
    marks INT
);
```

---

## 📥 Insert Sample Data

```sql
INSERT INTO students
(name, age, course, city, email, marks)
VALUES
('Nitin',21,'B.Tech','Delhi','nitin@gmail.com',85),
('Rahul',22,'BCA','Mumbai','rahul@gmail.com',75),
('Priya',20,'B.Tech','Pune','priya@gmail.com',90);
```

---

## 🔍 SQL Concepts Covered

### Data Definition Language (DDL)

- CREATE DATABASE
- CREATE TABLE
- ALTER TABLE
- DROP TABLE

### Data Manipulation Language (DML)

- INSERT
- UPDATE
- DELETE

### Data Query Language (DQL)

- SELECT
- DISTINCT
- LIMIT
- ORDER BY
- WHERE

### Filtering Operators

- AND
- OR
- NOT
- BETWEEN
- IN
- LIKE
- IS NULL
- IS NOT NULL

---

## 📊 Example Queries

### Top 3 Students

```sql
SELECT *
FROM students
ORDER BY marks DESC
LIMIT 3;
```

### Students from Delhi

```sql
SELECT *
FROM students
WHERE city='Delhi';
```

### Students with Marks Above 80

```sql
SELECT *
FROM students
WHERE marks > 80;
```

---

## 📸 Project Screenshots

Add screenshots here after running queries.

---

## 🎯 Learning Outcomes

After completing this project I learned:

- Database Design
- PostgreSQL Basics
- CRUD Operations
- Data Filtering
- Data Sorting
- Query Writing
- SQL Best Practices

---

## 👨‍💻 Author

Nitin Singh

Aspiring Data Analyst

GitHub:
https://github.com/nsr-dev-in

LinkedIn:
https://www.linkedin.com/in/nsr2k06/

---

## ⭐ Support

If you found this project useful, consider giving it a star.
