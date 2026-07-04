# Data Cleaning and Integrity Report

## Procedures Performed
- **Initial Audit:** Evaluated the raw/dirty financial transactions data column by column to identify inconsistencies, structural errors, and formatting discrepancies.
- **Column-by-Column Cleaning:** Systematically processed every feature to fix date formats, standardize numerical data, and handle missing values, while maintaining the original records intact without deletion.
- **Flagging & Formatting:** Rather than deleting ambiguous or invalid entries, specific flags and standard formats were introduced to preserve full data lineage.

## Data Cleaning Tools Used
- **OpenRefine:** Employed for initial data profiling, clustering textual values to handle minor typo variations, and column-by-column facet audits.
- **Python pandas Scripts:** Used automated scripts for scalable cleaning, explicit type casting (e.g., date conversion, monetary rounding), and adding conditional flag columns to mark data anomalies while keeping original values intact.
