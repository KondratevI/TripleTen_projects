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
- **Checked for missing values:** Identified and handled any missing data in the dataset.
- **Checked for duplicated values:** Detected and removed any duplicate rows to ensure data integrity.
- **Checked for incorrect column names:** Verified that column names were consistent and clear.
- **Checked for data type correspondence:** Ensured that each column had the correct data type (e.g., integers, floats, dates).
- **Checked for misprints:** Identified any errors or inconsistencies in data entries (such as spelling mistakes or wrong values).
- **Checked for wrong lower or higher cases:** Ensured text data was consistent in terms of letter casing (e.g., "Sales" vs. "sales").
- **Checked for outliers**: Identified any extreme values that could skew the results and decided how to handle them.
- **Corrected data:** Made necessary corrections to the data to ensure accuracy.
- **Deleted data:** Removed any data that could not be corrected or was irrelevant.
#### Step 2: Financial Analysis
- **Calculated total revenue by years and months:** Computed total revenue for each year and month, then plotted the corresponding graph.
- **Calculated total profit by years and months:** Computed total profit for each year and month, then plotted the corresponding graph.
- **Calculated total margin by years and months:** Calculated the total margin (profit/revenue) by year and month, then plotted the corresponding graph.
- **Calculated revenue by divisions by years and months:** Determined the revenue per division over time (yearly and monthly), then plotted the corresponding graph.
- **Calculated profit by divisions by years and months:** Calculated the profit per division by year and month, then plotted the corresponding graph.
- **Calculated margin by divisions by years and months:** Calculated the margin per division by year and month, then plotted the corresponding graph.
- **Calculated revenue by segments by years and months:** Determined the revenue per segment over time (yearly and monthly), then plotted the corresponding graph.
- **Calculated profit by segments by years and months:** Calculated the profit per segment by year and month, then plotted the corresponding graph.
- **Calculated margin by segments by years and months:** Calculated the margin per segment by year and month, then plotted the corresponding graph.
- **Calculated revenue by categories by years and months:** Computed revenue by categories over time (yearly and monthly), then plotted the corresponding graph.
- **Calculated profit by categories by years and months:** Computed profit by categories over time (yearly and monthly), then plotted the corresponding graph.
- **Calculated margin by categories by years and months:** Computed margin by categories over time (yearly and monthly), then plotted the corresponding graph.
- **Found the most profitable divisions, segments, and categories of the products:** Identified the best-performing parts of the business.
- **Found the least profitable divisions, segments, and categories of the products:** Identified the underperforming parts of the business.
- **Identified unprofitable divisions, segments, or categories of the products:** Determined if there were any areas that were not generating profit.
- **Provided recommendations:** Suggested improvements based on the analysis.
