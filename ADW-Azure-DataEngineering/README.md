**☁️End-to-End Azure Data Engineering Pipeline (AdventureWorks)**

**Overview**

This project implements a complete modern data engineering pipeline on Azure, using the AdventureWorks dataset. It follows the Medallion Architecture (Bronze → Silver → Gold) to transform raw data into analytics-ready insights and visualize them in Power BI.

**Architecture Summary**

Data Ingestion → Azure Data Factory\
Data Storage (Bronze Layer) → Azure Data Lake Storage Gen2\
Data Transformation (Silver Layer) → Azure Databricks\
Data Warehouse (Gold Layer) → Azure Synapse Analytics\
Visualization → Power BI (via Synapse SQL Endpoint)
![PrjArchitecture](https://github.com/user-attachments/assets/a5086d9b-ceae-48fe-ae97-d705c7f4573c)


**Tech Stack**

Azure Data Factory (ADF)\
Azure Data Lake Storage Gen2\
Azure Databricks (PySpark)\
Azure Synapse Analytics\
Power BI\
SQL (Synapse Serverless)

**Pipeline Workflow**

**🥉 Bronze Layer (Raw Data Ingestion)**\
Ingested ~10 tables from GitHub repository using Azure Data Factory\
Stored raw datasets in Azure Data Lake Gen2 (Bronze zone)\
Maintained original structure for traceability\
**🥈 Silver Layer (Data Transformation)**\
Cleaned and transformed data using Azure Databricks\
Performed:Data cleansing, aggregation, Joins across tables, Schema standardization\
Stored curated datasets in Silver layer
**🥇 Gold Layer (Data Warehouse)**\
Built data warehouse model in Azure Synapse Analytics\
Created external tables on transformed data\
Optimized data for analytics and reporting\
**📊 Power BI Integration**\
Connected Power BI to Synapse SQL Endpoint\
Built interactive dashboards for business insights

**📊 Key Outcomes**

Fully automated end-to-end ETL pipeline on Azure\
Implemented Medallion Architecture (Bronze, Silver, Gold)\
Enabled scalable analytics-ready data warehouse\
Delivered real-time BI dashboards using Power BI\
Improved data accessibility and reporting efficiency.
