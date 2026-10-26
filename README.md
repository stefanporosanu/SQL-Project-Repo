# 🗄️ SQL Data Analysis Projects

> **Data Technician Bootcamp | SQL | Supabase | Relational Databases & Data Analysis**

![SQL](https://img.shields.io/badge/SQL-Data%20Analysis-blue?style=flat-square)
![Supabase](https://img.shields.io/badge/Supabase-Database-green?style=flat-square)
![Database](https://img.shields.io/badge/Relational-Database-orange?style=flat-square)

---

## 🔎 Overview

This repository contains a collection of **SQL projects and exercises** completed during my Data Technician Bootcamp.

The work demonstrates practical experience creating and querying relational databases, filtering and sorting records, performing aggregations, grouping data and joining related tables to extract useful insights.

The projects use datasets including the **Northwind retail database** and a **World database**, providing experience analysing customer, product, order, supplier, geographic and demographic data.

---

## 📂 Projects Included

| Project | Focus |
|---|---|
| 🛍️ **Northwind Retail Database** | Analysing customers, products, orders, suppliers and sales-related data |
| 🌍 **World Database Analysis** | Exploring cities, countries, populations and geographic relationships |
| 🗃️ **Relational Database Design** | Understanding tables, primary keys, relationships and database structure |
| ☁️ **Supabase SQL Practice** | Creating databases and running SQL queries in a cloud database environment |

---

## 🛠️ SQL Skills & Techniques

### 🔍 Data Retrieval

Used `SELECT` statements to retrieve complete tables or specific columns from datasets.

```sql
SELECT CustomerName, City, Country
FROM Customers;
```

This allowed only the information required for a particular analysis to be returned.

---

## 🎯 Filtering with WHERE

The `WHERE` clause was used to filter records based on specific conditions.

Examples included:

- Customers from a particular country
- Customers from a specific city
- Products above or below a certain price
- Orders within specific date ranges
- Cities above a population threshold

```sql
SELECT *
FROM Customers
WHERE Country = 'Germany';
```

---

## ↕️ Sorting with ORDER BY

`ORDER BY` was used to organise query results and make patterns easier to identify.

Examples included:

- Products from lowest to highest price
- Products from highest to lowest price
- Customers sorted by country
- Cities ranked by population
- Countries ranked by life expectancy

```sql
SELECT ProductName, Price
FROM Products
ORDER BY Price DESC;
```

---

## 📊 Aggregations

Aggregate functions were used to summarise larger datasets.

Functions included:

| Function | Application |
|---|---|
| `COUNT()` | Counted records and unique values |
| `SUM()` | Calculated totals |
| `AVG()` | Calculated averages |
| `MIN()` | Identified minimum values |
| `MAX()` | Identified maximum values |

Example:

```sql
SELECT AVG(Price) AS AveragePrice
FROM Products;
```

---

## 📦 GROUP BY Analysis

`GROUP BY` was used to summarise data by categories and identify patterns within datasets.

Examples included:

- Counting occurrences by city name
- Analysing average population by country
- Grouping customer or geographic data
- Creating category-level summaries

```sql
SELECT Name, COUNT(*) AS Occurrences
FROM City
GROUP BY Name
ORDER BY Occurrences DESC;
```

This made it possible to move from individual records to aggregated analytical insights.

---

## 🔗 Table JOINs

SQL joins were used to combine related information stored across multiple tables.

For example, city data was linked with country data using matching country codes.

```sql
SELECT city.Name AS City,
       country.Name AS Country,
       country.Continent
FROM city
INNER JOIN country
    ON city.CountryCode = country.Code
WHERE country.Continent = 'Europe';
```

This demonstrated how relational databases can connect information across separate tables without duplicating data.

---

## 🛍️ Northwind Retail Analysis

The **Northwind database** was used to practise SQL using a realistic retail and sales dataset.

Tables included areas such as:

- 👥 Customers
- 🛒 Orders
- 📦 Products
- 🏷️ Categories
- 🚚 Suppliers
- 👔 Employees
- 📋 Order details
- 🚛 Shippers

Queries were used to explore questions such as:

- Which customers are based in a particular country?
- Which products are the most or least expensive?
- How many customers are located in a specific region?
- Which customers have placed orders?
- What is the average product price?
- What quantity of products has been ordered?

---

## 💡 Retail & Sales Insights

The SQL exercises demonstrated how queries can answer practical business questions.

Examples included:

✅ Identifying customers by location  
✅ Finding high-value and low-value products  
✅ Counting customers and orders  
✅ Analysing product prices  
✅ Retrieving customers who had made purchases  
✅ Summarising order quantities  
✅ Sorting products by price  
✅ Filtering orders by date  
✅ Combining information stored across related tables  

These techniques form the basis of using SQL for **sales reporting, customer analysis and operational decision-making**.

---

## 🌍 World Database Analysis

The World database was used to apply the same SQL skills to geographic and demographic data.

Analysis included:

- Counting cities within countries
- Finding the highest and lowest populations
- Ranking countries by life expectancy
- Identifying cities within population ranges
- Calculating average population
- Analysing population density
- Identifying capital cities
- Joining country and city tables
- Filtering results by continent

This demonstrated how SQL techniques can be applied to datasets outside of retail and sales.

---

## 🗃️ Relational Database Concepts

The bootcamp also introduced the principles behind relational database design.

This included:

- Tables
- Columns
- Rows
- Primary keys
- Foreign keys
- Relationships
- Reducing duplicated data
- Structuring data across related tables

The work reinforced why relational databases are more effective than storing large amounts of interconnected data in a single spreadsheet.

---

## ☁️ Supabase

SQL queries and database exercises were completed using **Supabase**.

This provided practical experience working with a hosted database environment and running SQL against structured relational tables.

Tasks included:

- Creating tables
- Loading database data
- Running SQL queries
- Testing filters and aggregations
- Querying multiple related tables
- Working with realistic datasets

---

## 🧠 Additional SQL Techniques

The exercises also included:

- `DISTINCT`
- `LIKE`
- `IN`
- `BETWEEN`
- `LIMIT`
- `AND`
- `OR`
- `NOT`
- Subqueries
- Column aliases using `AS`

Example:

```sql
SELECT ProductName, Price
FROM Products
WHERE Price BETWEEN 10 AND 20
ORDER BY Price;
```

---

## 💡 What I Practised

Through these projects, I developed practical experience in:

✅ Writing SQL queries from scratch  
✅ Retrieving specific columns using `SELECT`  
✅ Filtering data using `WHERE`  
✅ Sorting results using `ORDER BY`  
✅ Summarising data with aggregate functions  
✅ Grouping data with `GROUP BY`  
✅ Combining tables using `JOIN`  
✅ Using subqueries  
✅ Working with relational database structures  
✅ Analysing retail and sales datasets  
✅ Extracting useful business insights  
✅ Working with SQL in Supabase  

---

## 🎯 Key Skills

`SQL` • `Supabase` • `SELECT` • `WHERE` • `ORDER BY` • `GROUP BY` • `JOIN` • `INNER JOIN` • `COUNT` • `SUM` • `AVG` • `MIN` • `MAX` • `DISTINCT` • `LIKE` • `BETWEEN` • `Subqueries` • `Relational Databases` • `Retail Analysis` • `Sales Analysis`

---

## 📚 Project Context

These projects were completed as part of my **Data Technician Bootcamp** and form part of my developing data analytics portfolio.

The work focuses on practical SQL and database skills relevant to **Data Technician** and **entry-level Data Analyst roles**, including querying structured data, combining related tables, summarising information and extracting insights that can support business decisions.
