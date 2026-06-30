# dirty_financial_transactions

<details>
<summary>Before/After Comparison</summary>

<table>
<tr>
<th>Before</th>
<th>After</th>
</tr>
<tr>
<td>

![Before](extract%20fin%20ops%20history%20.png)

</td>
<td>

![After](finanance%20trans%20ops%20clean%20.png)

</td>
</tr>
</table>

</details>

### Structured Text Snippet Data Comparison
- **Before:** Contains raw unvalidated operational data with negative values, inconsistent strings (e.g., `pay pal`, `creditcard`), and missing status codes.
- **After:** Appends automated validation flags (`NEGATIVE_QUANTITY`, `NEGATIVE_PRICE`, `FORMAT_CORRECTED`, `MISSING_STATUS`) to systematically audit and log record anomalies.

### Core Data Integrity Fixes Applied
- **Format Standardization:** Normalized text inputs, dates, and category fields.
- **Constraint Enforcement:** Identified and flagged illogical negative metrics for quantity and price.
- **Completeness Auditing:** Marked and monitored missing fields to ensure full observability.
