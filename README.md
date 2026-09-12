# Retail Sales Data Cleaning & Transformation using Excel Power Query

## Project Overview

This project focuses on cleaning and transforming a messy retail sales dataset using **Microsoft Excel Power Query**.

The objective was to identify and resolve data-quality issues, handle missing and duplicate values, validate numerical data, standardize the dataset, and prepare clean and reliable data for further analysis.

## Dataset

The dataset contains retail transaction information with 11 columns:

* Transaction ID
* Customer ID
* Category
* Item
* Price Per Unit
* Quantity
* Total Spent
* Payment Method
* Location
* Transaction Date
* Discount Applied

## Tools Used

* Microsoft Excel
* Power Query

## Data Cleaning & Transformation Steps

1. Imported the raw dataset into Power Query.
2. Removed completely blank rows.
3. Renamed columns for consistency.
4. Removed duplicate Transaction IDs.
5. Applied **Trim** and **Clean** transformations to text columns.
6. Replaced missing Item values with `"Unknown"`.
7. Calculated missing Price Per Unit values using `Total Spent ÷ Quantity`.
8. Removed 604 records where both Quantity and Total Spent were missing.
9. Checked and corrected data types.
10. Validated transaction dates.
11. Checked Quantity, Price Per Unit, and Total Spent for invalid zero or negative values.
12. Validated Total Spent using `Price Per Unit × Quantity`.
13. Reviewed the final dataset using Power Query **Column Quality**.

## Data Quality Findings

* **1,213** Item values were initially blank.
* Missing Price Per Unit values were recovered using available transaction data.
* **604** records had both Quantity and Total Spent missing and were removed.
* Discount Applied contained **True, False, and missing values**.
* Transaction dates ranged from **January 1, 2022 to January 18, 2025**.
* No zero or negative values were found in Quantity, Price Per Unit, or Total Spent.
* Total Spent validation resulted in a **difference of 0**, confirming consistency between Price Per Unit, Quantity, and Total Spent.

## Final Result

After cleaning and validation, the final dataset contained **11,971 records**.

The cleaned dataset was loaded into Excel and is included in this repository.

## Dataset Source

The dataset was sourced from Kaggle:

**Retail Store Sales – Dirty for Data Cleaning**

[View Dataset on Kaggle](https://www.kaggle.com/datasets/ahmedmohamed2003/retail-store-sales-dirty-for-data-cleaning)

## Key Skills Demonstrated

* Data Cleaning
* Data Transformation
* Missing Value Handling
* Duplicate Removal
* Data Validation
* Data Type Management
* Excel Power Query
* Data Quality Assessment

## Author

Lovely Goyal

Aspiring Data Analyst

Skills: Excel | Power Query | SQL | Power BI

This project was created as part of my Data Analyst portfolio to demonstrate
practical data cleaning and transformation skills using Excel Power Query.

## License

This project is intended for educational and portfolio purposes.
