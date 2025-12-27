# Data Cleaning Portfolio Project: Sales Data in Pandas

## Project Overview
In this project, I performed end-to-end data cleaning on a messy sales dataset using Python's Pandas library. The goal was to transform raw, inconsistent data into a structured format ready for downstream analysis.

## The Problem
The raw dataset contained several common data integrity issues:
* **Duplicates**: Redundant transaction entries.
* **Missing Values**: Missing dates and quantities.
* **Formatting Issues**: Leading/trailing spaces and inconsistent capitalization in names.
* **Incorrect Data Types**: Currency symbols ($) making numeric columns act like text.
* **Mixed Date Formats**: Inconsistent date strings (YYYY-MM-DD vs DD-MM-YYYY).

## Cleaning Steps Taken
1. **Deduplication**: Removed identical rows to ensure transaction accuracy.
2. **Missing Value Handling**: Dropped rows missing critical dates and imputed missing quantities with 1.
3. **Text Normalization**: Used string methods to trim whitespace and standardize names to Title Case.
4. **Numeric Conversion**: Stripped currency symbols and used `pd.to_numeric` with coercion to handle non-numeric junk data.
5. **Date Standardization**: Unified mixed date strings into a standard datetime format.
6. **Type Casting**: Converted quantity to integers to optimize storage and readability.

## Tools Used
* **Python**
* **Pandas**
* **NumPy**

## How to Run
1. Clone the repository.
2. Ensure you have Pandas and NumPy installed (`pip install pandas numpy`).
3. Run `python clean_data.py`.
