# dirty_financial_transactions

<details>
<summary>Before/After Comparison</summary>

<img src="extract fin ops history .png" width="100%">
<img src="finanance trans ops clean .png" width="100%">

</details>

### Structured Text Snippet Data Comparison
- **Before:** Contains raw unvalidated operational data with negative values, inconsistent strings (e.g., `pay pal`, `creditcard`), and missing status codes.
- **After:** Appends automated validation flags (`NEGATIVE_QUANTITY`, `NEGATIVE_PRICE`, `FORMAT_CORRECTED`, `MISSING_STATUS`) to systematically audit and log record anomalies.

### Core Data Integrity Fix Applied
- **Format Standardization:** Normalized text inputs, dates, and category fields.
- **Constraint Enforcement:** Identified and flagged illogical negative metrics for quantity and price.
- **Completeness Auditing:** Marked and monitored missing fields to ensure full observability.
