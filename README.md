# DSA-Excel-Project-Documentation

This is where i started my Portfolio when taking my DSA Project

## Project: Amazon Product Case Study Analysis

### Objective 
Analyze Amazon product data to uncover trends in pricing, discounts, ratings, and customer reviews to support business decisions.

### Key Questions Explored  
1. What is the average discount by product category?  
2. Which categories have the highest-rated products?  
3. How do discounts impact sales (potential revenue)?  
4. What is the distribution of product ratings?

## 2. Data Cleaning & Preparation  
### Steps Taken  
 1. Removed Duplicates
- Used `Data → Remove Duplicates` to ensure no repeated entries.  
2. Handled Missing Values 
- Replaced blanks in `rating_count` with `0` using `=IF(ISBLANK(A2), 0, A2)`.  
3. Standardized Text & Numbers  
- Applied `=TRIM()` and `=PROPER()` to fix inconsistent product names.
