# 🧹 Data Cleaning & Preparation – Retail Store Sales

## 📌 Project Overview

This project was completed as part of my **SWYNEX Technologies Internship – Task 1: Data Cleaning & Preparation**.

The purpose of this project was to inspect a real-world retail sales dataset, identify common data-quality problems, clean and standardize the data, and prepare it for further analysis.

The dataset was cleaned using **Microsoft Excel**, and the final cleaned dataset was exported as a CSV file and uploaded to GitHub.

---

## 🎯 Objectives

The main objectives of this project were to:

- Identify missing values
- Detect and check duplicate records
- Verify data types
- Identify inconsistent categorical values
- Apply appropriate data-cleaning techniques
- Prepare the dataset for further analysis

---

## 📊 Dataset Information

**Dataset Name:** Retail Store Sales  
**Source:** Public Kaggle Dataset  
**Tool Used:** Microsoft Excel

The dataset contains **12,575 records** and **11 columns**.

### Dataset Columns

| Column | Description |
|---|---|
| Transaction ID | Unique identifier for each transaction |
| Customer ID | Identifier of the customer |
| Category | Product category |
| Item | Name of the item purchased |
| Price Per Unit | Price of one unit of the item |
| Quantity | Number of units purchased |
| Total Spent | Total amount spent in the transaction |
| Payment Method | Method used for payment |
| Location | Transaction location/channel |
| Transaction Date | Date of the transaction |
| Discount Applied | Indicates whether a discount was applied |

---

## 🔍 Data Quality Issues Identified

During the initial inspection, the following missing values were identified:

| Column | Missing Values |
|---|---:|
| Item | 1,213 |
| Price Per Unit | 609 |
| Quantity | 604 |
| Total Spent | 604 |
| Discount Applied | 4,199 |

The dataset was also checked for:

- Duplicate records
- Incorrect data types
- Inconsistent categorical values
- Invalid or unusual values

---

## 🛠️ Data Cleaning Process

### 1. Handling Missing Item Values

Missing values in the **Item** column were replaced with:

`unknown`

This allowed the records to be retained while clearly indicating that the original item information was unavailable.

---

### 2. Handling Missing Quantity Values

There were **604 missing values** in the Quantity column.

Instead of leaving these cells empty, statistical imputation was used.

The median of the available Quantity values was calculated in Excel using:

`=MEDIAN(F2:F12576)`

The calculated median was:

**6**

Therefore, the missing Quantity values were replaced with **6**.

Median imputation was selected because Quantity is a discrete numerical variable, and the median provides a reasonable central value without being strongly affected by extreme observations.

---

### 3. Handling Missing Price Per Unit Values

Where sufficient information was available, missing **Price Per Unit** values were calculated using the relationship:

**Price Per Unit = Total Spent ÷ Quantity**

The Excel formula used was:

`=G2/F2`

This calculation was applied only where the required Total Spent and Quantity values were available.

---

### 4. Handling Missing Total Spent Values

Where **Price Per Unit** and **Quantity** were available, missing **Total Spent** values were reconstructed using the relationship:

**Total Spent = Price Per Unit × Quantity**

The Excel formula used was:

`=E2*F2`

This approach used the existing relationship between the numerical columns instead of inserting an arbitrary estimated value.

Rows where the required information was not available were not assigned fabricated values.

---

### 5. Handling Missing Discount Applied Values

There were missing values in the **Discount Applied** column.

These missing values were replaced with:

`UNKNOWN`

The column was standardized to:

- TRUE
- FALSE
- UNKNOWN

This provides a consistent representation for missing categorical information.

---

### 6. Checking for Duplicate Records

The dataset was checked for duplicate records using Excel's **Remove Duplicates** feature across all columns.

**Result:** No exact duplicate rows were found.

---

### 7. Validating Data Types

Important columns were checked to ensure that they contained appropriate data types.

The following validations were performed:

| Column | Validation |
|---|---|
| Transaction Date | Verified as a valid Excel date |
| Quantity | Verified as numeric |
| Price Per Unit | Verified as numeric |
| Total Spent | Verified as numeric |

Excel's `ISNUMBER()` function was used to verify the numerical fields and date values.

---

### 8. Checking Data Consistency

The following categorical columns were reviewed for inconsistent values:

- Category
- Item
- Payment Method
- Location
- Discount Applied

Values were checked for spelling, formatting, and consistency.

The dataset did not contain major inconsistent categorical variations after cleaning.

---

## 📋 Data Cleaning Summary

| Data Quality Issue | Cleaning Method |
|---|---|
| Missing Item | Replaced with `unknown` |
| Missing Quantity | Median imputation using value `6` |
| Missing Price Per Unit | Calculated using Total Spent ÷ Quantity where possible |
| Missing Total Spent | Calculated using Price Per Unit × Quantity where possible |
| Missing Discount Applied | Replaced with `UNKNOWN` |
| Duplicate Records | Checked using Remove Duplicates |
| Incorrect Data Types | Validated using Excel |
| Inconsistent Values | Reviewed and standardized |

---

## 📈 Results

After completing the cleaning process:

- Missing Item values were replaced with a consistent placeholder.
- Missing Quantity values were filled using the median value of **6**.
- Missing Price Per Unit values were calculated where sufficient information was available.
- Missing Total Spent values were reconstructed using **Price Per Unit × Quantity** where sufficient information was available.
- Missing Discount Applied values were standardized as `UNKNOWN`.
- Duplicate records were checked and no exact duplicate rows were found.
- Numeric fields were validated.
- Transaction Date values were verified.
- Categorical values were reviewed for consistency.

The resulting dataset is more structured and suitable for further **Exploratory Data Analysis (EDA), visualization, dashboards, and analytics**.

---

## 🧰 Tools & Technologies Used

- **Microsoft Excel**
- **CSV**
- **GitHub**

### Excel Functions and Features Used

- `MEDIAN()`
- `ISNUMBER()`
- Arithmetic formulas
- Filters
- Remove Duplicates
- Data validation
- Data consistency checks

---

## 📁 Project Files

### `retail_store_sales_cleaned.csv`

The cleaned version of the retail sales dataset prepared for further analysis.

### `README.md`

Project documentation describing the dataset, identified data-quality issues, cleaning methods, and results.

---

## 🎓 Key Learning Outcomes

Through this project, I gained practical experience in:

- Data inspection and profiling
- Identifying missing values
- Statistical imputation
- Reconstructing calculated values
- Duplicate detection
- Data type validation
- Categorical data standardization
- Data quality checking
- Preparing datasets for further analysis
- Documenting a data-cleaning workflow

---

## ✅ Conclusion

This project provided practical experience in the **data preparation stage of the data analytics workflow**.

By identifying and addressing missing values, applying statistical imputation, reconstructing derived values, validating data types, checking duplicate records, and reviewing categorical consistency, the retail sales dataset was prepared for further analysis.

The project demonstrates the importance of **clean, consistent, and reliable data before performing analysis or creating dashboards and reports**.

---

## 👩‍💻 Author

**Dharani Machireddy**

**B.Tech – Artificial Intelligence & Data Science**

**SWYNEX Technologies Internship – Task 1**
