# SWYNEX Data Cleaning & Preparation

## Project Overview
This project focuses on cleaning and preparing a public retail sales dataset for data analysis.

## Dataset
The dataset contains retail transaction information such as:
- Transaction ID
- Customer ID
- Category
- Item
- Price Per Unit
- Quantity
- Total Spent
- Payment Method
- Location
- Transaction Date
- Discount Applied

## Data Cleaning Performed

The following data cleaning steps were performed using Microsoft Excel:

1. Identified missing values.
2. Recovered missing Item values using related transaction information.
3. Recovered missing Quantity values where possible using Price Per Unit and Total Spent.
4. Replaced unrecoverable missing Item values with `unknown`.
5. Replaced missing Discount Applied values with `UNKNOWN`.
6. Checked payment method values for consistency.
7. Checked location values for consistency.
8. Checked transaction dates and formatting.
9. Checked for duplicate records.
10. Created a cleaned dataset for further analysis.

## Tools Used
- Microsoft Excel
- GitHub

## Output
The cleaned dataset is available in:

`retail_store_sales_cleaned.csv`
