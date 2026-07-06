SQL Data Warehouse Project

📌 Overview

An end-to-end Data Warehouse project built using MySQL, implementing the Medallion Architecture (Bronze → Silver → Gold) to transform raw source data into clean, business-ready datasets for BI reporting.

🏗️ Architecture

Source Systems → Bronze → Silver → Gold → BI Reporting


Source: CRM and ERP systems (CSV files, 3 files each — 6 total)
Bronze Layer: Raw data ingestion
Silver Layer: Cleaned and standardized data
Gold Layer: Business-ready fact/dimension models exposed as views


🔹 Bronze Layer (Raw)


Created dedicated schema and tables with appropriate data types
Imported all 6 source CSV files into MySQL
Validated import accuracy via row count checks against source files


🔹 Silver Layer (Cleaned & Standardized)


Designed cleaned table schemas
Performed data quality checks on every table:

Null and duplicate checks on primary keys
Invalid values and extra spaces in other columns
Date format consistency



Used SQL functions: CAST, CHAR_LENGTH, CONCAT, SUBSTRING, DATE/DATETIME, IN/NOT IN
Loaded cleaned data using INSERT INTO ... SELECT


🔹 Gold Layer (Business-Ready)


Conducted data quality analysis aligned with business requirements
Chose schema design: Star Schema
Identified Fact and Dimension tables
Built relationships using joins
Exposed final models as views: gold.table_name


🛠️ Tech Stack


MySQL
Git/GitHub for version control


📊 Outcome

Clean, structured, analytics-ready data modeled for consumption by BI tools (e.g., Power BI, Tableau) for dashboarding and reporting.

🙏 Acknowledgment

Project inspired by Data with Bara
