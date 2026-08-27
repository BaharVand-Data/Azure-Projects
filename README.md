# ☁️ Azure Data Fundamentals (DP-900) Project
2
 
3
## 📖 Project Overview
4
 
5
This project was completed as part of the **Microsoft Azure Data Fundamentals (DP-900)** training course. It demonstrates foundational knowledge of cloud computing, relational and non-relational data solutions, data analytics, and modern Azure-based data architectures.
6
 
7
Using a combination of Azure services, I explored how data can be stored, ingested, processed, and analyzed to support business decision-making. The project included hands-on experience with **Azure SQL Database**, **Azure Storage Account**, **Azure Cosmos DB**, **Microsoft Fabric Lakehouse**, and **Eventstreams**.
8
 
9
---
10
 
11
## 🎯 Objectives
12
 
13
- Understand core cloud computing concepts and Azure data services.
14
- Work with both relational and non-relational data.
15
- Perform data ingestion using multiple Azure methods.
16
- Query and analyze datasets using SQL.
17
- Explore analytical workloads within Microsoft Fabric.
18
- Gain practical experience with modern data platform architectures.
19
 
20
---
21
 
22
## 🏗️ Technologies & Services Used
23
 
24
- Microsoft Azure
25
- Azure SQL Database
26
- Azure Storage Account
27
- Azure Cosmos DB
28
- Microsoft Fabric Lakehouse
29
- Microsoft Fabric Eventstreams
30
- Power BI
31
- SQL
32
 
33
---
34
 
35
## 🗄️ Relational Data with Azure SQL Database
36
 
37
Designed and queried relational databases to manage structured business data such as retail and sales information.
38
 
39
### Skills Demonstrated
40
 
41
- Creating and querying relational databases
42
- Understanding tables, keys, and relationships
43
- Data filtering and sorting
44
- Data aggregation and reporting
45
- Multi-table analysis using joins
46
 
47
### SQL Techniques Used
48
 
49
```sql
50
SELECT ProductName, SalesAmount
51
FROM Sales
52
WHERE SalesAmount > 1000
53
ORDER BY SalesAmount DESC;
54
```
55
 
56
```sql
57
SELECT ProductCategory,
58
SUM(SalesAmount) AS TotalSales
59
FROM Sales
60
GROUP BY ProductCategory;
61
```
62
 
63
```sql
64
SELECT c.CustomerName,
65
s.SalesAmount
66
FROM Customers c
67
JOIN Sales s
68
ON c.CustomerID = s.CustomerID;
69
```
70
 
71
**Key Concepts:**
72
- SELECT
73
- WHERE
74
- ORDER BY
75
- GROUP BY
76
- JOINs
77
- Aggregations
78
 
79
---
80
 
81
## 📦 Non-Relational Data Solutions
82
 
83
### Azure Storage Account
84
 
85
Worked with cloud-based storage services for managing unstructured and semi-structured data.
86
 
87
**Activities Included:**
88
- Storing CSV and JSON files
89
- Understanding Blob Storage
90
- Organising cloud-based datasets
91
- Exploring scalable storage solutions
92
 
93
### Azure Cosmos DB
94
 
95
Explored NoSQL database concepts through Azure Cosmos DB.
96
 
97
**Skills Developed:**
98
- Document-based data storage
99
- Working with JSON data
100
- Understanding scalability and partitioning
101
- Comparing relational vs. non-relational databases
102
 
103
---
104
 
105
## 📊 Analytics with Microsoft Fabric Lakehouse
106
 
107
Used Microsoft Fabric Lakehouse to explore modern analytical workloads and unified data storage.
108
 
109
### Activities Included
110
 
111
- Creating and managing Lakehouse environments
112
- Working with structured and unstructured data
113
- Exploring analytics and reporting workflows
114
- Understanding Data Lake and Data Warehouse concepts
115
 
116
### Data Formats
117
 
118
- CSV
119
- JSON
120
- Parquet
121
 
122
---
123
 
124
## ⚡ Data Ingestion
125
 
126
Explored various methods of bringing data into analytical environments.
127
 
128
### Microsoft Fabric Eventstreams
129
 
130
- Real-time data ingestion
131
- Event-driven architectures
132
- Streaming data processing
133
- Data movement into Fabric environments
134
 
135
### Additional Ingestion Methods
136
 
137
- File uploads
138
- Data pipelines
139
- ETL processes
140
- ELT processes
141
- Batch and near real-time ingestion
