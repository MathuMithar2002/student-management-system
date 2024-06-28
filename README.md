# student-management-system
# Library Management System

## Overview
The Library Management System is a simple project to manage a library's books, members, and loans. It allows librarians to add, update, delete, and view books and members, as well as manage the loans of books to members.

## Features
- Add, update, delete, and view books.
- Add, update, delete, and view members.
- Manage book loans (borrow and return books).

## Database Schema
The project uses a MySQL database with the following schema:

- **Books Table**
  - `book_id` (Primary Key)
  - `title`
  - `author`
  - `genre`
  - `published_year`

- **Members Table**
  - `member_id` (Primary Key)
  - `name`
  - `email`
  - `phone`

- **Loans Table**
  - `loan_id` (Primary Key)
  - `book_id` (Foreign Key)
  - `member_id` (Foreign Key)
  - `loan_date`
  - `return_date`

## Setup Instructions
Follow these steps to set up the Library Management System on your local machine:

### Prerequisites
- MySQL installed on your local machine.
- Python installed on your local machine.
- MySQL connector for Python (`mysql-connector-python`).

### Step 1: Create the Database and Tables
1. Open your MySQL client (e.g., MySQL Workbench) and create a new database called `LibraryDB`.

```sql
CREATE DATABASE LibraryDB;
USE LibraryDB;
