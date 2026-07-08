 
# Dirty Financial Transactions - Data Integrity System

[![Data Quality Solutions](https://img.shields.io/badge/Data_Quality-Solutions-blue.svg)](#)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](#)

An automated system designed to scan, isolate, and remediate anomalous or "dirty" transaction entries within financial data pipelines. This project focuses on maintaining strict system integrity, preventing data corruption propagation, and generating clean operational reports.

---

## 📌 Project Overview

Financial systems frequently ingest noisy data, duplicate logs, or intentionally corrupted transaction strings that compromise accounting accuracy. Similar to operational control systems that track stock metrics, prevent manual logging errors, and monitor leakage, this pipeline acts as an automated validation layer.

### Core Objectives
* **Automate Transaction Cleaning:** Programmatically flag invalid schemas, negative values where prohibited, and broken transaction chains.
* **Maintain Data Integrity:** Isolate "dirty" rows into secure error logs without disrupting downstream analytical processes.
* **Audit Reporting:** Generate structured metrics on data cleanliness, tracking error distribution types by source or date.

---

## 🚀 Key Features

* **Ingestion Guardrails:** Real-time checking against pre-defined data schemas and data types.
* **Anomaly Detection Isolation:** Identifies structural mismatches, duplicate processing IDs, and transactional timestamps out of chronological sequence.
* **Audit Log Generation:** Automatically saves clean datasets to primary storage and routes rejected entries into an isolated file structure for debugging.
* **System Integrity Reports:** Generates summaries detailing error rates, failure points, and data pipeline compliance levels.

---

## 🛠️ Tech Stack & Requirements

* **Language:** Python 3.8+
* **Libraries/Frameworks:** Pandas / NumPy / OpenRefine (for visual auditing)
* **Environment:** Virtual environment configuration included via `requirements.txt`

---

## 📖 Getting Started

### 1. Installation
Clone this repository to your local machine and navigate inside the project directory:
```bash
git clone [https://github.com/Datadog-995/Dirty-Financial-Transactions--Data-Integrity.git](https://github.com/Datadog-995/Dirty-Financial-Transactions--Data-Integrity.git)
cd Dirty-Financial-Transactions--Data-Integrity

<img width="687" height="150" alt="Screenshot - FINANCIAL TRANS DIRTY 2026-07-06 at 7 46 39 PM" src="https://github.com/user-attachments/assets/a0e4d774-5f0a-4bb3-8b7a-3c3f33edfef8" />

<img width="1230" height="344" alt="Screenshot 2026-07-07 at 11 33 20 PM" src="https://github.com/user-attachments/assets/f5c16e3d-fb41-4585-88dc-fd9377021dda" />

