# Task 5: SQL Joins (Inner, Left, Right, Full)

## Objective
Learn to combine data from multiple tables using different SQL join types: INNER JOIN, LEFT JOIN, RIGHT JOIN, and FULL JOIN.

## Tools Used
- DB Browser for SQLite / SQLiteStudio
- MySQL Workbench

## Contents
- `Task5-SQL_Joins.sql` → SQL script for Task 5  
- `customers.csv` and `orders.csv` → Sample datasets for practice  
- `screenshots/` → Final output screenshots  
- `README.md` → Project documentation  

---

## Tables Used

### Customers

| CustomerID | CustomerName | City      |
|------------|--------------|-----------|
| 1          | Alice        | Mumbai    |
| 2          | Bob          | Delhi     |
| 3          | Charlie      | Bangalore |
| 4          | Diana        | Hyderabad |

### Orders

| OrderID | CustomerID | Product  | Quantity | Price  |
|---------|------------|----------|----------|--------|
| 101     | 1          | Laptop   | 1        | 50000  |
| 102     | 2          | Mouse    | 2        | 500    |
| 103     | 1          | Keyboard | 1        | 1500   |
| 104     | 4          | Monitor  | 1        | 7000   |

---

## SQL Queries and Join Types

### 1. INNER JOIN  
Returns only rows where there is a match in both tables.


SELECT Customers.CustomerName, Orders.Product, Orders.Quantity
FROM Customers
INNER JOIN Orders ON Customers.CustomerID = Orders.CustomerID;

## LEFT JOIN

SELECT Customers.CustomerName, Orders.Product, Orders.Quantity
FROM Customers
LEFT JOIN Orders ON Customers.CustomerID = Orders.CustomerID;

##  RIGHT JOIN

SELECT Customers.CustomerName, Orders.Product, Orders.Quantity
FROM Customers
RIGHT JOIN Orders ON Customers.CustomerID = Orders.CustomerID;

## FULL JOIN

SELECT Customers.CustomerName, Orders.Product, Orders.Quantity
FROM Customers
FULL OUTER JOIN Orders ON Customers.CustomerID = Orders.CustomerID;

Author
**Name:** Bhargavi Thammina  
**Email:** bhargavithammina@gmail.com  
**LinkedIn:** [linkedin.com/in/bhargavi-thammina-846053263](https://linkedin.com/in/bhargavi-thammina-846053263)  
**GitHub:** [github.com/Bhargavi-Thammina](https://github.com/Bhargavi-Thammina)
---


