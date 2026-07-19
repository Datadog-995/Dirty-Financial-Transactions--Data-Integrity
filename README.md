# Data Integrity Audit: Financial Transactions

This repository contains an end-to-end audit and remediation pipeline for a dataset plagued by systemic data entry errors.

## Problem Solved: Data Auditing
The dataset contained significant integrity failures that I resolved to ensure report accuracy:
* **The "01/01/1900" Problem:** Thousands of rows contained default system date errors. I implemented a flagging system (`audited_dates`) to quarantine these records, preserving the audit trail for investigation.
* **Negative Financials:** I identified erroneous negative prices caused by system glitches, re-calculating values based on unit prices to restore financial integrity.
* **Missing Attributes:** Standardized "UNKNOWN" and "NaN" entries across categorical columns (Payment Methods, Locations) to ensure consistent grouping for business intelligence.

## Key Insights & Visualizations
*After cleaning, I generated the following reports to validate the dataset's integrity:*

![Revenue by Product](revenue_by_product.png)
![Payment Methods](payment_methods.png)
![Monthly Sales Trends](monthly_sales_trend.png)

## Repository Contents
* `raw_financial_transactions.csv`: The original, uncleaned source data.
* `CLEAN-Financial_Transactions.csv`: The finalized, cleaned dataset ready for analysis.
* `History-Openrefine-Financial_transactions.json`: Audit trail of transformation steps.
* `financial_Transactions_csv.ipynb`: The technical notebook used for verification.
the dataset's integrity:*

![Revenue by Product](https://raw.githubusercontent.com/Datadog-995/Dirty-Financial-Transactions--Data-Integrity/main/revenue_by_product.png)

![Payment Methods](https://raw.githubusercontent.com/Datadog-995/Dirty-Financial-Transactions--Data-Integrity/main/payment_methods.png)

![Monthly Sales Trends](https://raw.githubusercontent.com/Datadog-995/Dirty-Financial-Transactions--Data-Integrity/main/monthly_sales_trend.png)
