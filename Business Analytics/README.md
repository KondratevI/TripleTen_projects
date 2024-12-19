# Project - Business Analytics

### The goal

The goal of this project is to explore dataset, carry out analysis of the data and make recommendations.

#### The Data

The data was spread across three files:
- `sessions.csv`: each row corresponds to a user's session in the app
    - `'Uid'`: Unique identifier of the user
    - `'Device'`: User's device type
    - `'Start Ts'`: Session start date and time
    - `'End Ts'`: Session end date and time
    - `'Source Id'`: Identifier of the ad source the user came from
- `orders.csv`: each row corresponds to a user's order
    - `'Uid'`: Unique identifier of the user making the order
    - `'Buy Ts'`: Order date and time
    - `'Revenue'`: Yandex.Afisha's revenue from the order
- `costs.csv`: each row corresponds to daily marketing expenses for an ad source
    - `'source_id'`: Identifier of the ad source
    - `'dt'`: Date of the expense
    - `'costs'`: Marketing expenses for this ad source on the specified day


#### Process and Results

To do this I've done:

preprocess the data identifying and fillyng in missing values, identifying and remove duplicate values,
find out:
how many people use it every day, week, and month,
how many sessions are there per day,
what is the length of each session,
what's the user retention rate,
when do people start buying,
how many orders do they make during a given period of time,
what is the average purchase size,
how much money do they bring? (LTV),
how much money was spent? Overall, per source and over time,
how much did customer acquisition from each of the sources cost,
how worthwhile where the investments? (ROI),
create plots and heatmaps to show patterns.

The project was divided into three parts:
- **Profits & Losses:** Identified the biggest profit and loss centers, recommended products to stop selling, found the relationships between total numbers of sales and returns.
- **Advertising:** Identified the best states and months for advertising, calculating the return on ad spend ratio.
- **Returned Items:** Analyzed the return rates of products and examined the relationship between profit and return rates.
