# Project - A/B Testing

The data was spread across three files:

`/hypotheses_us.csv`: each row corresponds to a hypothesis
- `'Hypotheses'`: brief descriptions of the hypotheses
- `'Reach'`: user reach, on a scale of one to ten
- `'Impact'`: impact on users, on a scale of one to ten
- `'Confidence'`: confidence in the hypothesis, on a scale of one to ten
- `'Effort'`: the resources required to test a hypothesis, on a scale of one to ten. The higher the Effort value, the more resource-intensive the test.

`/datasets/orders_us.csv`: each row corresponds to a user's order
- `'transactionId'`: order identifier
- `'visitorId'`: identifier of the user who placed the order
- `'date'`: date of the order
- `'revenue'`: revenue from the order
- `'group'`: the A/B test group that the user belongs to
- 
`/visits_us.csv`: each row corresponds to user visits
- `'date'`: date
- `'group'`: A/B test group
- `'visits'`: the number of visits on the date specified in the A/B test group specified

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
- **Statistical significance of the conversion difference between groups (filtered data):** Tested the statistical significance on the filtered data.
- **Statistical significance of the average order size difference between groups (filtered data):** Tested the statistical significance on the filtered data.
#### Step 5: Conclusions and Recommendations
- Summarized the results of the tests and graphs.
- Drew conclusions on which group performed better.
- Provided recommendations for further improvements and testing.
