 # Student Management System

A simple **Java-based Student Management System** that allows users to **add, update, delete, and view** student records using a MySQL database as the backend.  
The project uses **Java Swing** for the GUI and **JDBC** for database connectivity.

## Features
- Add new student records
- Update existing student details
- Delete student records
- View all student records in a table format
- Simple and easy-to-use interface

## Technologies Used
- **Java (Swing + JDBC)**
- **MySQL Database**
- **MySQL Connector/J** (JDBC Driver)

## Requirements
1. Java JDK 8 or higher
2. MySQL installed locally
3. MySQL Connector/J JAR file (add it to your classpath)

## Database Setup
Run the following SQL commands in MySQL to set up the database:

```sql
CREATE DATABASE studentdb;
USE studentdb;

CREATE TABLE students (
    id INT PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(100) NOT NULL,
    roll_number VARCHAR(50) NOT NULL UNIQUE,
    course VARCHAR(100),
    contact VARCHAR(15)
);
