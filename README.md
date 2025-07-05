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
### Building the Data Warehouse

**Objective**

Develop a modern data warehouse using SQL Server to consolidate sales data, enabling analytical reporting and informed decision-making.

**Specifications**
- Data Sources: Import data from two source systems (ERP and CRM) provided as CSV files.
- Data Quality: Cleanse and resolve data quality issues prior to analysis.
- Integration: Combine both sources into a single, user-friendly data model designed for analytical queries.
- Scope: Focus on the latest dataset only; historization of data is not required.
- Documentation: Provide clear documentation of the data model to support both business stakeholders and analytics teams.



### BI: Analytics & Reporting

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
- SQL Server
- Draw.io
- Excel

## Data Modeling 
![data modeel](https://github.com/Ravina172/sql-data-warehouse-project/blob/main/Docs/data_model1.png)
The data warehouse uses a star schema to support business-level reporting and analytics. Dimensional modeling ensures efficient querying and usability across layers.

**Fact Table**
- fact_sales: Captures each sales transaction including references to customer, product, and location, with measures like revenue and quantity.

**Dimension Tables**
- dim_customer: Unified customer data from CRM and ERP, including demographics and join info
- dim_product: Merged product catalog across systems with standardized categories

##  ETL Process Breakdown
The pipeline follows the Medallion Architecture structure:

🟫 **Bronze Layer**
- Raw data loaded from CSV files with no transformation
- Maintains data fidelity for auditing and rollback

🟪 **Silver Layer**
- Cleansing: Removed duplicates, fixed data types, normalized fields
- Integration: Combined customer and product records from both CRM and ERP
- Modeled into structured fact/dim tables for analysis

🟨 **Gold Layer**
- Business metrics calculated: revenue, sales by region/product/customer
- Designed for dashboarding and self-serve reporting

![image](https://github.com/Ravina172/sql-data-warehouse-project/blob/main/Docs/data_integration1.png)

## Testing & Validation
Verified joins with expected record counts across fact/dimension tables
- Checked NULLs and duplicate keys
- Cross-validated Gold Layer metrics using pivot tables in Excel

## About-Me
I’m a data enthusiast with a passion for transforming raw data into meaningful insights that drive business decisions. This project is part of my ongoing journey to deepen my skills in data analytics and engineering. I'm continuously learning and exploring areas like data warehousing, BI tools, and scalable pipeline design.
<p align="left">
  <a href="https://www.linkedin.com/in/ravina-patidar-474a9b255/" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/>
  </a>
    </a>
  <a href="https://yourportfolio.com" target="_blank">
    <img src="https://img.shields.io/badge/Portfolio-157A6E?style=for-the-badge&logo=internet-explorer&logoColor=white" alt="Portfolio"/>
  </a>
  <a href="https://github.com/ravina172" target="_blank">
    <img src="https://img.shields.io/badge/GitHub-24292e?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/>
  </a>
  <a href="https://www.kaggle.com/ravinapatidar" target="_blank">
    <img src="https://img.shields.io/badge/Kaggle-004D99?style=for-the-badge&logo=kaggle&logoColor=white" alt="Kaggle"/>
  </a>
</p>


