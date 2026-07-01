


🏗 Workflow Architecture & Design Choices
The pipeline explicitly segregates visual text parsing from automated programmatic validation to optimize processing efficiency.

Phase 1: Exploration & Clustering (OpenRefine)
Design Choice: Text data is highly unpredictable due to human input variance. OpenRefine was selected for initial structural analysis because its key-collision and nearest-neighbor clustering algorithms quickly isolate text anomalies at scale.

Execution: Designed and committed customized GREL (General Refine Expression Language) expressions to strip out invisible formatting blocks and standardize raw currency notation layouts into strict fixed-decimal values.

Phase 2: Production Automation (Python & Pandas in Colab)
Design Choice: While OpenRefine excels at manual interactive cleaning, programmatic scripts are required for robust, repeatable batch processing.

Execution: Implemented an end-to-end Python script using Pandas within Google Colab. The script applies automated data constraints, checks database logic rules, logs processing anomalies, and isolates bad records into clean, observable flags without breaking the production runner.

How to Execute the Pipeline
The automated cleaning engine is fully contained within the script file located at:
scripts/cleaned_financial_transactions.ipynb

Open the notebook directly inside Google Colab, load your raw structural data file, and execute the runtime cells to generate a fully audited, production-ready transaction dataset.
