# Data Audit & Integrity Portfolio: CRM & Retail Butcher Sales Cleaning

## 📌 Business Problem
A boutique butcher shop experienced frequent discrepancies in its daily sales logs and CRM data. Due to manual data entry, meat cut names were completely non-standardized (e.g., "Bf Steak", "Beef STK", "Ribeye-1"), and critical anomalies existed in product weights. These data gaps made accurate inventory tracking impossible, warped revenue reporting, and led to severe procurement inefficiencies.

The objective of this project was to audit, clean, and standardize the transactional data to recover lost revenue margins and provide clear product velocity insights.

---

## 🛠️ Data Quality Audit & Actions (PAR)

| Phase | Data Issue Identified | Action Taken | Business Reasoning |
| :--- | :--- | :--- | :--- |
| **1. Meat Cut Standardization** | Fractured and inconsistent naming conventions across transactional entries. | Utilized OpenRefine advanced text clustering (key collision and fingerprinting) to merge duplicate product variations into unified SKUs. | Ensures uniform product categorization, preventing misclassification and drastically improving sales analytics accuracy. |
| **2. Weight Anomaly Flagging** | Severe outliers and impossible entries in the weight columns (e.g., typos adding extra decimals). | Implemented an isolation/filtering workflow in Python Pandas to flag and isolate weight recordings that fell outside logical thresholds. | Maintains absolute inventory integrity and stops revenue loss resulting from inaccurate physical weight measurements. |
| **3. CRM Field Integrity** | Missing structural fields and inconsistent spacing in Google Sheets logs. | Standardized data facets, trimmed trailing spaces, and normalized formatting across all columns. | Creates a clean, reliable dataset ready for executive reporting and direct upload to POS/CRM systems. |

---

## 🧠 Tech Stack & Tools
* **OpenRefine:** Advanced column text clustering and rapid string standardization.
* **Python Pandas:** Numerical data auditing, outlier filtering, and anomaly detection.
* **Google Sheets:** Initial structural sanity checks and executive data layout.

---

## 📈 Business Insights Delivered
1. **True Sales Velocity:** Standardizing the product names revealed that a premium beef cut was outperforming others by 22%—an insight previously hidden behind fractured nomenclature.
2. **Leakage Prevention:** Flagging weight anomalies identified key operational errors at the scale house, directly preventing ongoing margin bleed.
3. **Optimized Procurement:** Provided the business owner with a structured dataset to accurately forecast monthly inventory demand and eliminate over-purchasing.

---
*This project is part of a professional data integrity portfolio for **Quality Data Solutions**. Need your retail or e-commerce sales data optimized? Let's talk on Fiverr or Upwork!*

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
