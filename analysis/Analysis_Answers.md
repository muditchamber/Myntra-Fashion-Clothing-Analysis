# Myntra Fashion Clothing — Analysis & Answers

## 1. Data Analysis

### Q1. Overall Average Original Price for Products with Ratings Greater Than 4

**Result:** ₹1,966.67

**Excel Formula:**

`=AVERAGEIF(Table2[Ratings],">4",Table2[OriginalPrice (in Rs)])`

---

### Q2. Number of Products with Discount Greater Than 50% OFF

**Result:** 232,123 products

**Excel Formula:**

`=COUNTIF(Table2[Discount_Percentage],">50%")`

---

### Q3. Number of Products Available in Size M

**Result:** 656 products

**Excel Formula:**

`=COUNTIF(Table2[SizeOption],"M")`

---

## 2. Product Classification

A new column named `Label_product` was created to classify products according to their discount percentage.

### Classification Rule

- **High Discount:** Discount greater than 50%
- **Low Discount:** Discount of 50% or less

---

## 3. Product Lookup

### Q4. Product ID: 11226634

VLOOKUP and XLOOKUP were used to retrieve product information.

| Field | Result |
|---|---|
| Product ID | 11226634 |
| Brand | Maniac |
| Price | ₹1,199 |
| Rating | 3.9 |

Both VLOOKUP and XLOOKUP returned the same product information.

---

## 4. INDEX + MATCH

### Q5. Discount Price for Product ID 6744434

**Result:** ₹599

**Excel Formula:**

`=INDEX(Table2[DiscountPrice (in Rs)],MATCH(6744434,Table2[Product_id],0))`

---

## 5. Nested XLOOKUP

### Q6. Retrieve Any Column Detail Using Product ID

The nested XLOOKUP method was used to retrieve a selected column value based on Product ID.

**Example:**

| Product ID | Requested Column | Result |
|---|---|---|
| 2296012 | Ratings | 3.9 |

This approach allows a user to dynamically retrieve information from different columns using a Product ID.

---

## 6. Excel Functions Used

The following Excel functions were used in this project:

- AVERAGEIF
- COUNTIF
- VLOOKUP
- XLOOKUP
- INDEX
- MATCH

---

## 7. Key Results

| Analysis | Result |
|---|---:|
| Average Original Price for Rating > 4 | ₹1,966.67 |
| Products with Discount > 50% | 232,123 |
| Products Available in Size M | 656 |
| Product 11226634 Brand | Maniac |
| Product 11226634 Price | ₹1,199 |
| Product 11226634 Rating | 3.9 |
| Product 6744434 Discount Price | ₹599 |
| Product 2296012 Rating | 3.9 |

---

## 8. Conclusion

This analysis demonstrates the use of Microsoft Excel for product-level analysis, conditional calculations, discount classification, and data retrieval.

The project combines data analysis functions with lookup techniques to extract meaningful information from a large fashion retail dataset.
