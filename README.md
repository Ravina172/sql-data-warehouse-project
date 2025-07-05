# Data Warehouse And Analytics Project

## Project Overview 
In this project, I built an end-to-end data warehouse that takes raw operational data and turns it into clean, structured, and analysis-ready datasets. I followed Medallion Architecture, structured into Bronze, Silver, and Gold layers.The objective was to build an end-to-end data pipeline that supports scalable, reliable analytics.
Key components of the project include:
1. Data Architecture: Designing a Modern Data Warehouse Using Medallion Architecture Bronze, Silver, and Gold layers.
2. ETL Pipelines: Extracting, transforming, and loading data from source systems into the warehouse.
3. Data Modeling: Developing fact and dimension tables optimized for analytical queries.
4. Analytics & Reporting: Develop SQL-based analytics to deliver detailed insights.
  
## Data Architecture
In this project i used Medallion Architecture Bronze, Silver and Gold layers:
![image](https://github.com/Ravina172/sql-data-warehouse-project/blob/main/Docs/data_architecture%202.png)
1. Bronze Layer: Stores raw data as-is from the source systems. Data is ingested from CSV Files into SQL Server Database.
2. Silver Layer: This layer includes data cleansing, standardization, and normalization processes to prepare data for analysis.
3. Gold Layer: Houses business-ready data modeled into a star schema required for reporting and analytics.

## Objective
1. **Building the Data Warehouse**
**Objective**
Develop a modern data warehouse using SQL Server to consolidate sales data, enabling analytical reporting and informed decision-making.

**Specifications**
- Data Sources: Import data from two source systems (ERP and CRM) provided as CSV files.
- Data Quality: Cleanse and resolve data quality issues prior to analysis.
- Integration: Combine both sources into a single, user-friendly data model designed for analytical queries.
- Scope: Focus on the latest dataset only; historization of data is not required.
- Documentation: Provide clear documentation of the data model to support both business stakeholders and analytics teams.

2. **BI: Analytics & Reporting**
**Objective**
Develop SQL-based analytics to deliver detailed insights into:
  - Customer Behavior
  - Product Performance
  - Sales Trends
These insights empower stakeholders with key business metrics, enabling strategic decision-making.

## Dataset
The dataset for this project simulates raw data ingested from two operational source systems — CRM and ERP — each contributing key business entities. These sources contain overlapping but differently structured information, reflecting real-world data integration challenges.

📁**Source Systems Overview**
- CRM System: Focused on customer relationships and sales transactions.
Includes:
  - customer_info.csv – Basic customer records (name, contact, join date)
  - product_info.csv – Product catalog details
  - sales_info.csv – Sales transactions with customer and product references

- ERP System: Focused on operations and logistics.
Includes:
  - customer_info.csv – Extended customer data including birthday and age
  - location_info.csv – Regional and warehouse location details
  - product_info.csv – Operational product data with differing schema (e.g., SKU codes, vendor info)

## Tools

