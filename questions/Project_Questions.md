# Project Questions

## A. Data Cleaning and Preparation
1. Check for duplicate values in the dataset and remove them.
2. Standardize the `DiscountOffer` column to a single format, ensuring all values are uniform.
3. Identify rows where both `DiscountPrice` and `DiscountOffer` are null and fill `DiscountPrice` with the average discount price of the respective category.
4. Replace all null values in `SizeOption` column with the text `Not Available`.

## B. Data Analysis
1. Calculate the overall average original price for products with ratings greater than 4.
2. Count the number of products with a discount offer greater than 50% OFF.
3. Count the number of products available in size `M`.
4. Create a new column to label the products as `High Discount` if the discount offer is greater than 50% OFF, otherwise label them as `Low Discount`.

## C. Data Retrieval and Lookup
1. Use VLOOKUP/XLOOKUP to find the product brand, price, and rating of the product with Product ID `11226634`.
2. Find the `DiscountPrice` for the product with the Product ID `6744434` using INDEX and MATCH functions.    
3. Utilize nested XLOOKUP to find any column's detail of a product using its Product ID.
