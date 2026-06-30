# 💰 Financial Transaction Data Integrity Pipeline

<details>
<summary>Before/After Comparison</summary>

<img src="extract fin ops history .png" width="100%">
<img src="finanance trans ops clean .png" width="100%">

</details>

### Structured Text Snippet Data Comparison

| Column | Before (Raw Unvalidated) | After (Validated & Flagged) |
| :--- | :--- | :--- |
| **Payment_Method** | `pay pal`, `creditcard` | `PayPal`, `Credit Card` (Format Standardized) |
| **Quantity** | `-5` | `5` / Flagged `NEGATIVE_QUANTITY` |
| **Price** | `-150.00` | `150.00` / Flagged `NEGATIVE_PRICE` |
| **Status_Code** | *[Blank]* | Flagged `MISSING_STATUS` |

### Core Data Integrity Fixes Applied

- **Format Standardization:** Normalized text inputs, dates, and category fields to ensure absolute uniformity across transaction logging systems.
- **Constraint Enforcement:** Identified and flagged illogical negative metrics for quantity and price to preserve ledger consistency.
- **Completeness Auditing:** Systematically marked and monitored missing fields to ensure full lifecycle observability and compliance.
