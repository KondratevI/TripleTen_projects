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

#### Process and Results

To achieve the results, I have:

- Preprocessed the data by identifying and filling in missing values, as well as identifying and removing duplicate entries.
- Split the source data into a training set, validation set, and test set.
- Tested various classifiers on the validation set:
  - `DecisionTreeClassifier` with different `max_depth` hyperparameters.
  - `RandomForestClassifier` with various combinations of `n_estimators` and `max_depth` hyperparameters.
  - `LogisticRegression with different solver hyperparameters.
- Applied the best-performing hyperparameters to the test set.
- Made conclusions based on the results.

The project was divided into three parts:
- **Profits & Losses:** Identified the biggest profit and loss centers, recommended products to stop selling, found the relationships between total numbers of sales and returns.
- **Advertising:** Identified the best states and months for advertising, calculating the return on ad spend ratio.
- **Returned Items:** Analyzed the return rates of products and examined the relationship between profit and return rates.
