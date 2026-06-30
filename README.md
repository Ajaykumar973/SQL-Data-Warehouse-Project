#  SQL Data Warehouse Project

A modern **SQL Data Warehouse** solution built using **Microsoft SQL Server** that implements the **Medallion Architecture (Bronze, Silver, and Gold layers)**. This project demonstrates an end-to-end ETL pipeline that ingests raw data from multiple business systems, transforms it into standardized datasets, and delivers business-ready data for analytics and reporting.

---

##  Project Overview

The objective of this project is to design and implement a scalable, maintainable, and efficient data warehouse capable of supporting business intelligence and analytical workloads.

The solution follows a layered architecture that separates raw ingestion, data transformation, and business presentation, ensuring high data quality, simplified maintenance, and improved reporting performance.

---

##  Architecture

The data warehouse follows the **Medallion Architecture**, consisting of three logical layers.

##  Solution Architecture

![SQL Data Warehouse Architecture](DWH_Architecture.png)

---

###  Bronze Layer – Raw Data

The Bronze layer serves as the landing zone for source data.

**Responsibilities**

- Load raw data from CRM and ERP systems
- Preserve source data without modification
- Support full data refresh
- Store historical raw records

**Objects**

- Tables
- Stored Procedures

---

###  Silver Layer – Cleaned & Standardized Data

The Silver layer transforms raw data into a clean, consistent, and reliable format.

**Transformations**

- Data cleansing
- Data standardization
- Data normalization
- Data enrichment
- Derived columns
- Data validation

**Objects**

- Tables
- Stored Procedures

---

###  Gold Layer – Business Data

The Gold layer provides curated datasets optimized for analytics and reporting.

**Responsibilities**

- Business logic implementation
- Data integration
- Aggregations
- Analytical modeling

**Objects**

- Views
- Fact Tables
- Dimension Tables
- Star Schema

---

##  Data Pipeline

```text
CSV Files (CRM / ERP)
          │
          ▼
Bronze Layer (Raw Data)
          │
          ▼
Silver Layer (Cleaned & Standardized Data)
          │
          ▼
Gold Layer (Business-Ready Data)
          │
          ▼
BI Dashboards • SQL Analytics • Machine Learning
```

---

##  Project Structure

```text
SQL-Data-Warehouse/
│
├── datasets/
│   ├── crm/
│   └── erp/
│
├── scripts/
│   ├── bronze/
│   ├── silver/
│   ├── gold/
│   └── stored_procedures/
│
├── docs/
│   └── architecture.png
│
└── README.md
```

---

##  Technologies Used

- Microsoft SQL Server
- SQL
- SQL Server Management Studio (SSMS)
- Stored Procedures
- Views
- ETL Processes
- Data Warehousing
- Star Schema Modeling

---

##  Key Features

- End-to-End ETL Pipeline
- Multi-Source Data Integration
- Layered Medallion Architecture
- Automated Data Loading
- Data Cleansing & Validation
- Business Logic Implementation
- Star Schema Design
- Business-Ready Reporting Layer

---

## 📊 Business Value

This solution enables organizations to:

- Centralize enterprise data
- Improve data quality and consistency
- Reduce reporting complexity
- Deliver trusted datasets for analytics
- Support business intelligence initiatives
- Enable scalable reporting and decision-making

---

##  Use Cases

- Business Intelligence
- Executive Dashboards
- Ad-Hoc SQL Analysis
- Data Analytics
- KPI Reporting
- Machine Learning

---

##  Solution Architecture

![SQL Data Warehouse Architecture]()

---

##  Future Enhancements

- Incremental Data Loading
- Change Data Capture (CDC)
- SQL Server Agent Automation
- Power BI Dashboard Integration
- Data Quality Monitoring
- Azure Data Factory Integration
- Azure Synapse Analytics Migration

---

##  Author

**Ajay Kumar**

