# 📚 Online Bookstore Database - SQL Practice Project

A comprehensive MySQL database project implementing an online bookstore management system with complex queries demonstrating various SQL concepts and techniques.

## 🎯 Project Overview

This project contains a complete relational database schema for an online bookstore, including table creation, data manipulation, and a collection of SQL queries ranging from basic to advanced complexity.

## 📊 Database Schema

### Tables

#### 1. **Books**
- `Book_ID` - Primary Key (Serial)
- `Title` - VARCHAR(100)
- `Author` - VARCHAR(100)
- `Genre` - VARCHAR(50)
- `Published_Year` - INT
- `Price` - NUMERIC(10, 2)
- `Stock` - INT

#### 2. **Customers**
- `Customer_ID` - Primary Key (Serial)
- `Name` - VARCHAR(100)
- `Email` - VARCHAR(100)
- `Phone` - VARCHAR(15)
- `City` - VARCHAR(50)
- `Country` - VARCHAR(150)

#### 3. **Orders**
- `Order_ID` - Primary Key (Serial)
- `Customer_ID` - Foreign Key
- `Book_ID` - Foreign Key
- `Quantity` - INT
- `Order_Date` - DATE
- `Total_Amount` - NUMERIC(10, 2)

## 🔍 SQL Queries Implemented

### Basic Queries
1. Retrieve all books in the "Fiction" genre
2. Find books published after 1950
3. List all customers from Canada
4. Show orders placed in November 2023
5. Retrieve total stock of books available
6. Find the most expensive book

### Intermediate Queries
7. Show customers who ordered more than 1 quantity
8. Retrieve orders where total amount exceeds $20
9. List all distinct genres available
10. Find the book with the lowest stock
11. Calculate total revenue from all orders

### Advanced Queries
1. **Total books sold per genre** - Using JOINs and GROUP BY
2. **Average price of Fantasy books** - Aggregate functions with filtering
3. **Customers with at least 2 orders** - Subqueries and COUNT with HAVING
4. **Top 5 most expensive Fantasy books** - Sorting and limiting results
5. **Total quantity of books sold by each author** - Multi-table joins with aggregation
6. **Cities with customers spending over $30** - Complex joins with GROUP BY and HAVING
7. **Customer who spent the most** - Aggregation with sorting
8. **Stock remaining after fulfilling orders** - Subqueries with calculations

## 🛠️ Technologies Used

- **Database**: MySQL 8.0
- **Tool**: MySQL Workbench
- **SQL Features**:
  - DDL (Data Definition Language)
  - DML (Data Manipulation Language)
  - JOINs (INNER, LEFT)
  - Aggregate Functions (SUM, AVG, COUNT)
  - Subqueries
  - GROUP BY & HAVING clauses
  - ORDER BY & LIMIT

## 📁 Project Structure

```
online-bookstore-db/
│
├── schema/
│   └── create_tables.sql          # Database schema creation
│
├── queries/
│   ├── basic_queries.sql          # Simple SELECT statements
│   ├── intermediate_queries.sql   # Queries with aggregation
│   └── advanced_queries.sql       # Complex multi-table queries
│
├── screenshots/
│   ├── schema_design.png
│   ├── basic_queries.png
│   ├── intermediate_queries.png
│   └── advanced_queries.png
│
└── README.md
```

## 🚀 How to Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/online-bookstore-db.git
   cd online-bookstore-db
   ```

2. **Create the database**
   ```sql
   CREATE DATABASE OnlineBookStore;
   USE OnlineBookStore;
   ```

3. **Run the schema file**
   ```bash
   mysql -u root -p OnlineBookStore < schema/create_tables.sql
   ```

4. **Execute queries**
   ```bash
   mysql -u root -p OnlineBookStore < queries/basic_queries.sql
   ```

## 📈 Key Learnings

- Designed normalized database schema with proper relationships
- Implemented various types of SQL joins for multi-table queries
- Used aggregate functions for business analytics
- Applied filtering and sorting for efficient data retrieval
- Practiced subqueries and complex conditional logic
- Optimized queries for performance

## 🎓 Skills Demonstrated

- Database Design & Normalization
- SQL Query Writing & Optimization
- Data Analysis & Reporting
- Relational Database Concepts
- Business Logic Implementation

## 📸 Screenshots

### Database Schema
![Schema Design](screenshots/schema_design.png)

### Query Execution
![Query Results](screenshots/basic_queries.png)

## 🤝 Contributing

Feel free to fork this project and submit pull requests for any improvements!

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 📧 Contact

**Your Name**
- GitHub: [@yourusername](https://github.com/yourusername)
- LinkedIn: [Your Profile](https://linkedin.com/in/yourprofile)
- Email: your.email@example.com

---

⭐ If you found this project helpful, please give it a star!
