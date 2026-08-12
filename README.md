# KNIME ETL Pipeline

## Overview
An end-to-end ETL pipeline built in KNIME Analytics Platform for cleaning and loading customer data.

## Pipeline Steps
1. **CSV Reader** – Import dirty customer data
2. **Missing Value** – Impute missing values (Unknown, Not Available, Mean)
3. **Duplicate Row Filter** – Remove duplicate records
4. **String Manipulation** – Proper Case formatting
5. **Column Rename** – Standardize column names
6. **Row Filter** – Validate data (Age > 0, Salary > 0)
7. **PostgreSQL Connector + DB Writer** – Load to PostgreSQL

## Results
- **Rows before:** 10
- **Rows after dedup:** 9
- **Rows after validation:** 6
- **Target database:** hamia_db
- **Target table:** customers_clean

## Tech Stack
- KNIME Analytics Platform
- PostgreSQL
- pgAdmin
- Python (for data generation)

## Screenshots
Screenshots of each node configuration are included in the word doc.

## Author
Sajeela Noor
