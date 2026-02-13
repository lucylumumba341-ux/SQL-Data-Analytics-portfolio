# Retail Sales Analysis: SQL to Interactive Dashboard

## Project Overview
This project demonstrates an end-to-end data pipeline. I extracted raw sales data using **SQL**, performed advanced data cleaning in **Excel**, and built an interactive **Pivot Table Dashboard** to visualize regional sales performance.

---

## Phase 1: Data Extraction (SQL)
I developed a relational database in MySQL to store and manage customer and transaction records.
* **Task**: Created tables and populated them with raw data using `CREATE` and `INSERT` statements.
* **Interface**: Managed the extraction process through MySQL Workbench.

![SQL Workbench Setup](1_SQL_WORKBENCH_EXTRACTION.png)

---

## Phase 2: Identifying Inconsistencies & Data Cleaning
Before analysis, I identified several data quality issues in the raw export, including messy text, extra spaces, and inconsistent date formats.

![Raw Inconsistencies](2_RAW_DATA_INCONSISTENCIES.png)

### Cleaning Steps Taken:
* **Text Standardization**: Applied `=PROPER(TRIM())` to fix irregular capitalization and extra spaces in names.
* **Date Repair**: Resolved mixed date delimiters (periods vs. slashes) using the Text-to-Columns wizard to ensure chronological accuracy.
* **Deduplication**: Identified and removed duplicate rows to ensure data integrity.

![Cleaned Dataset](3_CLEAN_DATASET.png)

---

## Phase 3: Data Visualization & Insights
I utilized **Pivot Tables** and **Pivot Charts** to extract meaningful business insights from the cleaned dataset.

### Key Findings:
* **Regional Leaders**: The **Central** region generated the highest revenue, exceeding **$100,049**.
* **Interactivity**: Built-in **Slicers** allow stakeholders to filter by **Region** and **Status** instantly.
  

![Pivot Analysis](4_PIVOT_TABLE_ANALYSIS.png)
![Interactive Dashboard](5_INTERACTIVE_DASHBOARD.png)

---

## Technical Skills Used
| Tool | Application |
| :--- | :--- |
| **SQL** | Database creation, data insertion, and extraction |
| **Excel** | Data cleaning (PROPER, TRIM, Text-to-Columns) |
| **Data Viz** | Pivot Tables, Pivot Charts, and Interactive Slicers |

## How to View the Project
1. **Download the Dataset**: You can access the finalized Excel report here: [RETAIL_SALES_PERFORMANCE_ANALYSIS.xlsx](./RETAIL_SALES_PERFORMANCE_ANALYSIS.xlsx)
2. **Interact**: Open the file in Excel to use the Slicers and explore the automated charts.
3. **SQL Source**: The raw data extraction logic and table schemas are located in the .sql files within this repository.


# SQL Business Intelligence Portfolio

This repository contains SQL-based data analysis projects focused on transforming raw data into actionable business insights.

## 🛒 Project 1: Ecommerce Revenue & Growth Analysis
**Business Goal:** Track monthly revenue and identify growth trends to evaluate business health.
### # Key Skills: SQL Window Functions (LAG), CTEs, and Arithmetic Growth Calculations
### # Results: Successfully identified a 105% revenue increase between January and February.

![Ecommerce Analysis](ECOMMERCE%20REVENUE%20AND%20GROWTH%20ANALYSIS.png)

---

## 📦 Project 2: Inventory Optimization & Stock Alerts
**Business Goal:** Minimize stockouts by automating reorder warnings based on inventory levels.
### # Key Skills: CASE Statements, Conditional Logic, and Data Filtering
### # Results: Created an automated flagging system for items below safety stock levels.

![Inventory Analysis](INVENTORY%20OPTIMIZATION%20&%20STOCK%20ANALYSIS.png)

---

## 👥 Project 3: HR Salary Benchmarking & People Analytics
**Business Goal:** Analyze departmental pay structures to ensure internal equity.
### # Key Skills: PARTITION BY, Aggregations, and Salary Variance Analysis
### # Results: Compared individual salaries against departmental averages to highlight potential pay gaps.

![HR Analysis](HR%20SALARY%20BENCHMARKING%20&%20PEOPLE%20ANALYTICS.png)






