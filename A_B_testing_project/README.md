# Project - A/B Testing

The data was spread across three files:
- `hypotheses_us.csv`: each row corresponds to a user's session in the app
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
