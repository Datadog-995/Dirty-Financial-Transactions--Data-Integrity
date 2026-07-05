# Data Cleaning and Integrity Report

The core technology stack used to inspect, audit, and clean the datasets includes **OpenRefine**, **Python Pandas**, and **Google Sheets**. All code and scripts are included in the repository to verify the cleaning steps.

## Procedures Performed
- **Initial Audit:** Evaluated the raw/dirty financial transactions data column by column to identify inconsistencies, structural errors, and formatting discrepancies.
- **Column-by-Column Cleaning:** Systematically processed every feature to fix date formats, standardize numerical data, and handle missing values, while maintaining the original records intact without deletion.

## Scripts
A new directory named `scripts` contains automation scripts for cleaning and data integrity:
- `data_cleaner.py`: A sample Python cleaning script designed to automate the process of cleaning dirty financial transaction data and maintaining data integrity.
