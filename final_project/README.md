# Final Project

### The goal

Finding the most profitable and the less profitable divisions, segments and categories of the products.

#### The Data
It was provided a backup of the database in the SQLite format no CSV files will be provided.
The condition of the project was оnly use connections to the database itself, and not to load the whole database to CSV.

The data was spread across six tables:
- `dim_customer`: contains customer-related data.
- `dim_product`: contains product-related data
- `fact_pre_discount`: contains pre-invoice deductions information for each product
- `fact_manufacturing_cost`: contains the cost incurred in the production of each product
- `fact_gross_price`: contains gross price information for each product
- `fact_sales_monthly`: contains monthly sales data for each product.




### Process and Results

#### Step 1: Data Preprocessing
- **Handled missing values:** Identified and filled in missing values in key columns (orders, visits, group, order size, price).
- **Removed duplicates:** Checked for and removed duplicate rows to avoid distorting the analysis results.
#### Step 2: Visualization
- **Cumulative revenue by group:** Plotted the cumulative revenue for both groups.
- **Cumulative average order size by group:** Plotted the cumulative average order size.
- **Relative difference in cumulative average order size between groups:** Plotted the difference in average order size between groups A and B.
- **Scatter plot of orders per user:** Plotted the number of orders per user.
- **Scatter plot of order prices:** Plotted the order prices.
- **Daily conversion rates for both groups:** Plotted the daily conversion rates for both groups.
#### Step 3: Calculations
- **Conversion rate for each group:** Calculated the conversion rate for each group (the ratio of orders to visits per day).
- **95th and 99th percentiles for orders per user:** Calculated the percentiles for the number of orders.
- **95th and 99th percentiles for order prices:** Calculated the percentiles for the order prices.
#### Step 4: Statistical Analysis
- **Statistical significance of the conversion difference between groups (raw data):** Tested whether the conversion rates between the groups were statistically significant using a t-test.
- **Statistical significance of the average order size difference between groups (raw data):** Tested whether the average order size difference between the groups was statistically significant.
