# Project - Machine Learning

### The goal

The goal of this project is to explore datasets, find the best model with the best hyperparameters that will pick the right mobile plan for users of the mobile carrier.

#### The Data

- `'сalls'`: number of calls
- `'minutes'`: total call duration in minutes
- `'messages'`: number of text messages
- `'mb_used'`: Internet traffic used in MB
- `'is_ultra'`: plan for the current month (Ultra - 1, Smart - 0)

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
