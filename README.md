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


## 3. Key Excel Techniques Applied 
| Task                    | Method Used                              | Formula/Tool |
|---------------------|--------------------------------------|------------------|
| Unique Product Count    | PivotTable                               | `Distinct Count` |
| Average Discount        | PivotTable                               | `=AVERAGE()`     |
| Rating Distribution     | Histogram (Data Analysis Toolpak)        | `=FREQUENCY()`   |
| Potential Revenue       | Calculated Field in PivotTable           | `=actual_price * rating_count` |
| Price Buckets           | Conditional Grouping                     | `=IF(A2<200, "<₹200", IF(A2<=500, "₹200-500", ">₹500"))` |


## 4. Insights & Visualizations  
### Key Findings  
- Boat is the product with the highest number of reviews at (68).
- Cables & Accessories had the highest average discount (55%), but lower average ratings (4.1/5) compared to Smart TVs (4.3/5).  
- Electronics generated the highest potential revenue due to high `actual_price × rating_count`.  
- Products priced ₹500 had the most reviews, indicating strong customer engagement.


  ### Charts Created  
1. Bar Chart: Average Discount by Category  
   - Finding: Office products had deeper discounts than Electronics.  
2. Scatter Plot: Rating vs. Discount %  
   - Finding: No strong correlation—high discounts didn’t always mean low ratings.  
3. Pie Chart: Price Bucket Distribution  
   - Finding: 61% of products were under ₹500. 


## 5. Recommendations 
For Marketing Teams:  
- Leverage high discounts in Cables & Accessories to drive sales.  
- Highlight top-rated Electronics in promotions (avg. rating 4.3/5).  

For Pricing Strategy:  
- Test moderate discounts (30-40%) for high-revenue categories (e.g., Electronics).


  ## 6. Appendix  
### Sample Data Structure 
| Column             | Description                          | Example          |
|---------------------|--------------------------------------|------------------|
| `product_id`        | Unique product identifier            | B07JW9H4J1       |
| `category`          | Product category (e.g., Electronics)      | Electronics           |
| `discounted_price`  | Sale price (₹)                       | 399              |
| `actual_price`      | Original price (₹)                   | 1099             |
| `rating`            | Customer rating (1-5)                | 4.2              |
| `rating_count`      | Number of reviews                    | 24,269           |


### Skills Demonstrated 
- Data Cleaning  
- PivotTables & Advanced Formulas  
- Data Visualization   
- Business Insights Generation 

## Below are the images containing the Pivot table and Dashboard 
![IMG-20250704-WA0005](https://github.com/user-attachments/assets/9a721b0e-3bce-4dc6-8d7e-eec5428c0937)

![IMG-20250704-WA0006](https://github.com/user-attachments/assets/6bb16c38-1c1f-4a9c-9aaa-f8d66979baf6)

![IMG-20250704-WA0007](https://github.com/user-attachments/assets/41759e85-75ae-4e38-9129-75f2610d4339)

