# 🧹 Data Cleaning & Preparation – Retail Store Sales

## 📌 Project Overview

This project was completed as part of my **SWYNEX Technologies Internship – Task 1: Data Cleaning & Preparation**.

The objective of this task was to take a real-world retail sales dataset and prepare it for further analysis by identifying and handling:

- Missing values
- Duplicate records
- Incorrect data types
- Inconsistent categorical values
- Data quality issues

The dataset was cleaned using **Microsoft Excel**, and the final cleaned dataset was exported as a CSV file and uploaded to GitHub.

---

## 📊 Dataset

**Dataset:** Retail Store Sales  
**Source:** Public Kaggle Dataset

The dataset contains **12,575 records** and **11 columns**.

### Columns

| Column | Description |
|---|---|
| Transaction ID | Unique transaction identifier |
| Customer ID | Customer identifier |
| Category | Product category |
| Item | Product/item name |
| Price Per Unit | Price of one unit of the product |
| Quantity | Number of units purchased |
| Total Spent | Total amount spent in the transaction |
| Payment Method | Method used for payment |
| Location | Transaction location/channel |
| Transaction Date | Date of the transaction |
| Discount Applied | Whether a discount was applied |

---

## 🔍 Data Quality Issues Identified

During the initial inspection, the following missing values were identified:

| Issue | Count |
|---|---:|
| Missing Item | 1,213 |
| Missing Price Per Unit | 609 |
| Missing Quantity | 604 |
| Missing Total Spent | 604 |
| Missing Discount Applied | 4,199 |

The dataset was also checked for duplicate records, incorrect data types, and inconsistent categorical values.

---

## 🛠️ Data Cleaning Performed

### 1. Missing Item Values

Missing values in the **Item** column were replaced with:

`unknown`

This provided a consistent placeholder while preserving the affected records.

---

### 2. Missing Quantity Values

The missing values in the **Quantity** column were handled using **median imputation**.

The median of the available Quantity values was calculated using:

```excel
=MEDIAN(F2:F12576)
