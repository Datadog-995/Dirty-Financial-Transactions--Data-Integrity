## Quality Data Solutions: Financial Transaction Data Cleaning & Audit

This repository contains a comprehensive data cleaning pipeline for corporate financial transaction logs. It demonstrates how to transform raw, inconsistent data into a structured format using **OpenRefine**, **Python Pandas**, and **Google Sheets**, with all code and scripts provided to verify the cleaning steps.

### 📊 Repository Structure & Components

### 1. Raw Dataset (raw_data folder)
- **Status:** Untouched / Raw Input Data
- **Description:** The original, uncleaned financial logs containing missing values, inconsistent date formatting, and unstandardized numerical entries.

### 2. Cleaned Output (financial_Transactions_Cleaned.csv)
- **Status:** Pristine / Production-Ready Output
- **Description:** The final polished dataset. All missing values are addressed, numerical formats are standardized, whitespace is stripped, and formatting anomalies have been fully removed.

### 3. Automation Scripts (scripts/data_cleaner.py)
- **Status:** Programmatic Audit Footprint
- **Description:** Contains the Python Pandas scripts utilized during the data scrubbing phase to automate the cleaning process.

### 🛠️ Data Cleaning Footprint

The core data integrity steps applied to this dataset include:
- **Text Standardization:** Applied whitespace trimming and standardized formatting across all text-based fields.
- **Data Auditing & Imputation:** Flagged anomalous entries, handled missing values programmatically, and restructured date formats to ensure accurate downstream calculations.
- **Formatting:** Restructured the file into a clean, strictly formatted CSV ready for direct database upload or BI tool ingestion.
