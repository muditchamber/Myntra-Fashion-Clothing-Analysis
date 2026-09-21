# Myntra Fashion Clothing — EDA Report

## 1. Project Overview

This project focuses on cleaning, preparing, and analyzing a Myntra fashion clothing dataset using Microsoft Excel.

The project covers data cleaning, discount analysis, product analysis, and Excel lookup functions.

---

## 2. Project Objectives

The main objectives of this project are:

- Clean and prepare the dataset.
- Handle duplicate and missing values.
- Standardize discount-related information.
- Analyze product prices, ratings, discounts, and sizes.
- Classify products based on discount percentage.
- Retrieve product information using Excel lookup functions.

---

## 3. Data Cleaning and Preparation

The following data-cleaning tasks were performed:

### 3.1 Duplicate Values

Duplicate records were checked and removed from the dataset.

### 3.2 Discount Offer Standardization

The `DiscountOffer` column was standardized so that discount values follow a consistent format.

### 3.3 Missing Discount Price

Rows where both `DiscountPrice` and `DiscountOffer` were null were identified.

For these records, `DiscountPrice` was filled using the average discount price of the respective product category.

### 3.4 Missing Size Information

Null values in the `SizeOption` column were replaced with:

`Not Available`

---

## 4. Data Analysis

The following analysis was performed:

### 4.1 Average Original Price

The overall average original price was calculated for products with ratings greater than 4.

### 4.2 Products with More Than 50% Discount

The number of products having a discount offer greater than 50% OFF was calculated.

### 4.3 Products Available in Size M

The number of products available in size `M` was calculated.

### 4.4 Discount Classification

A new column named `Label_product` was created.

Products were classified as:

- `High Discount` — Discount greater than 50%
- `Low Discount` — Discount of 50% or less

---

## 5. Data Retrieval and Lookup

Excel lookup functions were used to retrieve product-level information.

### 5.1 VLOOKUP / XLOOKUP

VLOOKUP/XLOOKUP was used to find the following information for Product ID `11226634`:

- Product Brand
- Price
- Rating

### 5.2 INDEX and MATCH

INDEX and MATCH functions were used to find the `DiscountPrice` for Product ID `6744434`.

### 5.3 Nested XLOOKUP

Nested XLOOKUP was used to retrieve column-level details for a product based on its Product ID.

---

## 6. Excel Functions Used

The project uses Excel functions and features including:

- VLOOKUP
- XLOOKUP
- INDEX
- MATCH
- Average calculations
- Conditional logic
- Data cleaning
- Missing-value handling
- Data classification

---

## 7. Project Outcome

The project demonstrates practical use of Microsoft Excel for:

- Data cleaning
- Data preparation
- Exploratory data analysis
- Product-level analysis
- Discount analysis
- Lookup and retrieval operations

The analysis provides a structured approach to working with a large fashion retail dataset.

---

## 8. Conclusion

This project demonstrates an end-to-end Excel-based data analysis workflow, starting from data cleaning and preparation and progressing to analysis and product-level data retrieval using Excel lookup functions.
