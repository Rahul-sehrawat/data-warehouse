# data-warehouse

The objective of this project was to build a scalable and centralized Data Warehouse using SQL Server, where all relevant data sources could be cleaned, structured, and integrated. This setup aims to support efficient business intelligence, reporting, and strategic decision-making by ensuring data consistency, quality, and accessibility.

## Dataset Overview

The dataset used for this project consists of six CSV files, each containing critical business data from various departments:

- CustomerInfo.csv – Contains customer IDs, names, and core details.
- CustomerInfo.csv – Contains customer IDs, names, and core details.
- ProductInfo.csv – Includes product IDs, names, prices, and descriptions.
- SaleDetails.csv – Records of sales transactions with references to customers and products, including quantity and transaction dates.
- CustomerDemographics.csv – Includes customer gender and date of birth for demographic analysis.
- CustomerLocation.csv – Provides the geographic information of customers (country).
- ProductCategory.csv – Contains product categories and subcategories for classifying sales and inventory data.

## Data Warehouse Architecture

The project followed the Medallion architecture model to ensure data traceability, quality, and scalability. Each layer of the architecture served a clear purpose:

- Bronze Layer: Ingests raw ERP and CRM data from CSV files into staging tables in SQL Server.
- Silver Layer: Performs data cleaning, transformation, type standardization, and joins to normalize records.
- Gold Layer: Contains the final star schema, with well-modeled fact and dimension tables for fast querying.


