# SWYNEX Data Cleaning & Preparation – Retail Sales Dataset

## 📌 Project Overview

This project was completed as part of my Data Analyst internship at SWYNEX Technologies.

The objective of this task was to clean, transform, validate, and prepare a public retail sales dataset for further data analysis.

The dataset contains transaction-level retail sales information including customer details, product categories, prices, quantities, payment methods, locations, transaction dates, and discount information.

---

## 🎯 Objectives

The key objectives of this project were:

- Identify missing and invalid values
- Handle missing values appropriately
- Identify and handle duplicate records
- Check data consistency
- Correct data formatting and data types
- Validate numerical values using logical calculations
- Prepare a clean dataset for further analysis

---

## 📊 Dataset

**Dataset:** Retail Store Sales Dataset

**Type:** Public Dataset

### Main Columns

| Column | Description |
|---|---|
| Transaction ID | Unique identifier for each transaction |
| Customer ID | Identifier for the customer |
| Category | Product category |
| Item | Product/item name |
| Price Per Unit | Price of one unit |
| Quantity | Number of units purchased |
| Total Spent | Total transaction amount |
| Payment Method | Method used for payment |
| Location | Online or In-store |
| Transaction Date | Date of transaction |
| Discount Applied | Whether a discount was applied |

---

## 🧹 Data Cleaning Performed

The dataset was cleaned using **Microsoft Excel**.

### 1. Missing Values
- Identified missing values across important columns.
- Recovered values where they could be logically derived.
- Used `unknown` for Item values that could not be reliably recovered.
- Used `UNKNOWN` for unavailable Discount Applied values.

### 2. Data Validation
- Checked relationships between Price Per Unit, Quantity, and Total Spent.
- Verified that calculated values were logically consistent.

### 3. Consistency Checks
- Checked Payment Method values.
- Checked Location values.
- Checked Category and Item formatting.
- Checked Transaction Date formatting.

### 4. Duplicate Check
- Checked the dataset for duplicate records using Excel's **Remove Duplicates** feature.

### 5. Final Dataset
After cleaning and validation, the processed dataset was exported as a CSV file for further analysis.

---

## 🛠️ Tools Used

- Microsoft Excel
- GitHub
- CSV

---

## 📁 Project Files

- `retail_store_sales_cleaned.csv` – Cleaned dataset
- `README.md` – Project documentation

---

## 📈 Outcome

The raw retail sales dataset was cleaned and prepared for further data analysis.

This task provided practical experience in:

- Data cleaning
- Missing-value handling
- Data validation
- Data consistency checking
- Duplicate detection
- Excel-based data preparation
- GitHub project documentation

---

## 👩‍💻 Author

**Dharani Machireddy**

B.Tech – Artificial Intelligence & Data Science

---

## 🔗 Project Repository

This repository contains the cleaned dataset and documentation for the SWYNEX Data Cleaning & Preparation task.
