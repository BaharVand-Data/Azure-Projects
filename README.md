# ☁️ Azure Data Fundamentals (DP-900) Project

## 📝 Overview

This project was completed as part of the **Microsoft Azure Data Fundamentals (DP-900)** training course and demonstrates foundational knowledge of cloud computing, relational and non-relational data solutions, data analytics, and modern Azure-based data architectures.

Using a combination of Azure services, I explored how data is stored, ingested, processed, and analysed to support business decision-making. The project provided hands-on experience with **Azure SQL Database**, **Azure Storage Account**, **Azure Cosmos DB**, **Microsoft Fabric Lakehouse**, and **Eventstreams**.

---

## 🎯 Project Objectives

✅ Understand core cloud computing concepts and Azure data services

✅ Work with both relational and non-relational data solutions

✅ Perform data ingestion using batch and real-time Azure methods

✅ Query and analyse structured datasets using SQL

✅ Explore modern analytical workloads within Microsoft Fabric Lakehouse

✅ Gain practical experience with end-to-end data platform architectures

---

## 📸 Cloud Architecture Overview

<p align="center">

<img src="https://images.unsplash.com/photo-1551288049-bebda4e38f71?q=80&w=1000&auto=format&fit=crop" alt="Azure Cloud Data Architecture" width="900" />

</p>

---

## 🗄️ Relational Data with Azure SQL Database

I designed and queried relational databases to manage structured business data, including retail transactions and customer records.

### ✔️ Skills Demonstrated

- Creating and managing relational databases in Azure
- Defining tables, primary/foreign keys, and schema relationships
- Data filtering, sorting, and multi-table analysis using joins
- Performing aggregations for executive reporting

### 📸 Query Execution Examples

<p align="center">

<img src="https://images.unsplash.com/photo-1460925895917-afdab827c52f?q=80&w=1000&auto=format&fit=crop" alt="Azure SQL Query Execution" width="800" />

</p>

### 🧮 Sample SQL Queries

```sql
-- Filtering high-value sales
SELECT ProductName, SalesAmount
FROM Sales
WHERE SalesAmount > 1000
ORDER BY SalesAmount DESC;

-- Categorical aggregation
SELECT ProductCategory,
       SUM(SalesAmount) AS TotalSales
FROM Sales
GROUP BY ProductCategory;

-- Multi-table relational join
SELECT c.CustomerName,
       s.SalesAmount
FROM Customers c
JOIN Sales s
  ON c.CustomerID = s.CustomerID;
