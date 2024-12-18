# TripleTen Sprint 4 Project - Data Visualization with Tableau

### The goal

The goal is to review the superstore’s operations and increase its profitability. For each question, I should prepare an individual visualization that justifies my conclusion.

#### The Data


- `'Order ID'`: ID number that uniquely identifies each order
- `'Order Date'`:
- `'Ship Date'`:
- `'Ship Mode'`:
- `'Customer ID'`: ID number that uniquely identifies each customer account
- `'Customer Name'`:
- `'Segment'`:
- `'Country/Region'`:
- `'City'`:
- `'State'`:
- `'Postal Code'`:
- `'Region'`:
- `'Product ID'`: ID number that uniquely identifies each product
- `'Category'`:
- `'Sub-Category'`:
- `'Product Name'`:
- `'Sales'`:
- `'Quantity'`:
- `'Discount'`:
- `'Profit'`:




- `instacart_orders.csv`: each row corresponds to one order on the Instacart app
    - `'order_id'`: ID number that uniquely identifies each order
    - `'user_id'`: ID number that uniquely identifies each customer account
    - `'order_number'`: the number of times this customer has placed an order
    - `'order_dow'`: day of the week that the order placed (which day is 0 is uncertain)
    - `'order_hour_of_day'`: hour of the day that the order was placed
    - `'days_since_prior_order'`: number of days since this customer placed their previous order
- `products.csv`: each row corresponds to a unique product that customers can buy
    - `'product_id'`: ID number that uniquely identifies each product
    - `'product_name'`: name of the product
    - `'aisle_id'`: ID number that uniquely identifies each grocery aisle category
    - `'department_id'`: ID number that uniquely identifies each grocery department category
- `order_products.csv`: each row corresponds to one item placed in an order
    - `'order_id'`: ID number that uniquely identifies each order
    - `'product_id'`: ID number that uniquely identifies each product
    - `'add_to_cart_order'`: the sequential order in which each item was placed in the cart
    - `'reordered'`: 0 if the customer has never ordered this product before, 1 if they have
- `aisles.csv`
    - `'aisle_id'`: ID number that uniquely identifies each grocery aisle category
    - `'aisle'`: name of the aisle
- `departments.csv`
    - `'department_id'`: ID number that uniquely identifies each grocery department category
    - `'department'`: name of the department

The data is provided by TripleTen, who took it from Kaggle and modified it.

#### The Process

I first explored the dataset to find and fix missing and duplicate values, and I merged DataFrames from different sources. Finally, I analyzed the data using visualizations and pivot tables.

### Results

Taking the time to explain my results at each step was a key element in this process, and this was my first attempt at doing it. I wrote an introduction and conclusion that outlined what I did, and made suggestions for Instacart to consider in the future.

Please have a look at the Jupyter Notebook included for a full description of results.
