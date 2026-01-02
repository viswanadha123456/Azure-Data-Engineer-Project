# Azure-Data-Engineer-Project
This project demonstrates an end-to-end data engineering pipeline built from scratch using modern Azure data technologies.

Project Description
In this project, I take you through an End-to-End Data Engineering solution, where I leverage powerful technologies like:
Azure Data Factory
Azure Data Lake Storage (ADLS Gen2)
Azure Databricks
Apache Spark (PySpark)
👉 Databricks is used both for data processing and as the data warehouse, storing curated datasets in Delta format for analytics.
Architecture Overview
The project follows the Medallion Architecture implemented fully in Databricks:
Bronze Layer – Raw data ingestion
Silver Layer – Cleaned and transformed data
Gold Layer – Analytics-ready curated data
All layers are stored in Azure Data Lake and managed using Delta Lake in Databricks.
Data Ingestion
Data is ingested from source systems using Azure Data Factory
Pipelines are scheduled and monitored.
Bronze Layer (Raw Data)
Raw data is stored in Azure Data Lake
Minimal transformations applied
Silver Layer (Cleaned Data)
Data is cleaned, validated, and transformed using Databricks & PySpark
Stored in Delta format

Repository Structure
├── adf/
│   └── pipelines/
├── databricks/
│   └── notebooks/
├── data/
│   ├── bronze/
│   ├── silver/
│   └── gold/
└── README.md
