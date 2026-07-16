# E-Commerce Data Integrity & Automation Services

**Overview**
This repository serves as a functional portfolio demonstrating automated data ingestion, multi-page web scraping, and ledger formatting tailored for e-commerce and retail suppliers. The automated pipelines contained here transform messy, unstandardized data into clean, tax-ready CSV ledgers.

**Core Capabilities**
* **Automated Web Scraping:** Python-based web agents (`BeautifulSoup`, `requests`) designed to politely navigate multi-page e-commerce catalogs, bypassing static limits to extract competitor pricing and product data at scale.
* **Data Integrity & Formatting:** End-to-end cleaning workflows utilizing Pandas to strip anomalous text (e.g., rogue currency symbols), handle null values, and standardize date/time formats for financial modeling.
* **Cloud Automation:** Continuous integration pipelines built with GitHub Actions to schedule and execute data-cleaning scripts automatically.

**Featured Projects**
1.  **Brazilian E-Commerce Logistics Audit:** A comprehensive cleanup of a massive, multi-table retail dataset, structuring raw sales, customer, and shipping records into pristine, relational analytical outputs.
2.  **Bakery & Butcher Supplier Ledger:** An end-to-end data integrity project that transformed messy, inconsistent local sales records into a strictly formatted, calculable financial ledger.
3.  **Automated Price Extraction:** A dynamic scraping script that navigates paginated storefronts to harvest and immediately format raw pricing strings into pure float values for instant Excel compatibility. 

**Data Visualizations**
![Total Revenue Bar Chart](https://quickchart.io/chart?c={type:'bar',data:{labels:['Premium%20Beef%20Cuts','Artisan%20Bread','Poultry','Pastries','Pork','Specialty%20Cakes'],datasets:[{label:'Revenue',data:[45200,31500,28400,24100,19800,15600]}]}})
