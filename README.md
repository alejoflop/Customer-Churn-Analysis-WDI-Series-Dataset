# Customer Churn Analysis — WDI Series Dataset

An end-to-end data analytics and business intelligence solution designed to analyze customer activity, identify key churn drivers, and build predictive risk metrics using transactional and usage data from the `WDIseries` dataset.

---

## 📌 Project Overview

Customer churn significantly impacts revenue growth and customer lifetime value. This project establishes an end-to-end data pipeline and diagnostic analytics framework to:
1. Process and clean raw usage/transactional series data (`WDIseries.csv`).
2. Define customer churn logic and engineer behavioral risk features.
3. Model activity into a SQL-based Star Schema data mart.
4. Deliver interactive executive Power BI dashboards with actionable customer retention insights.

---

## 🛠️ Repository Structure

```text
customer-churn-analysis/
│
├── data/
│   ├── raw/                 # Raw datasets (WDIseries.csv) - [Git-ignored if >100MB]
│   └── cleaned/             # Processed datasets ready for staging
│
├── notebooks/               # Jupyter Notebooks for EDA & ETL
│   └── 01_data_cleaning_eda.ipynb
│
├── sql/                     # Modular SQL scripts (Database, Staging, Star Schema)
│   ├── 01_database_and_staging.sql
│   ├── 02_indexing_and_verification.sql
│   └── 03_star_schema_views.sql
│
├── powerbi/                 # Power BI templates (.pbit) and executive PDFs
│
├── docs/                    # Architecture diagrams & metric definitions
│   └── churn_metrics_dictionary.md
│
├── .gitignore               # Excludes raw data files, local envs, checkpoints
├── README.md                # Main project documentation
└── requirements.txt         # Python library dependencies
