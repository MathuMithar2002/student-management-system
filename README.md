# Student Management System

## Overview
The Student Management System is a simple project to manage student records and course enrollments. It allows administrators to add, update, delete, and view student information and courses, as well as manage the enrollment of students in courses.

## Features
- Add, update, delete, and view students.
- Add, update, delete, and view courses.
- Enroll students in courses.
- View enrollments.

## Database Schema
The project uses a MySQL database with the following schema:

- **Students Table**
  - `student_id` (Primary Key)
  - `name`
  - `email`
  - `phone`
  - `dob` (date of birth)

- **Courses Table**
  - `course_id` (Primary Key)
  - `course_name`
  - `course_description`

- **Enrollments Table**
  - `enrollment_id` (Primary Key)
  - `student_id` (Foreign Key)
  - `course_id` (Foreign Key)
  - `enrollment_date`

## Setup Instructions
Follow these steps to set up the Student Management System on your local machine:

### Prerequisites
- MySQL installed on your local machine.
- Python installed on your local machine.
- MySQL connector for Python (`mysql-connector-python`).

### Step 1: Create the Database and Tables
1. Open your MySQL client (e.g., MySQL Workbench) and create a new database called `StudentDB`.

```sql
CREATE DATABASE StudentDB;
USE StudentDB;
