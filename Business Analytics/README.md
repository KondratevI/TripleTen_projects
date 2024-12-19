# Project - Business Analytics

### The goal

The goal of this project is to explore datasets, find the best model with the best hyperparameters that will pick the right mobile plan for users of the mobile carrier.

#### The Data

- `'сalls'`: number of calls
- `'minutes'`: total call duration in minutes
- `'messages'`: number of text messages
- `'mb_used'`: Internet traffic used in MB
- `'is_ultra'`: plan for the current month (Ultra - 1, Smart - 0)

#### Process and Results

To do this I've done:

- preprocess the data identifying and filling in missing values, identifying and remove duplicate values,
- split the source data into a training set, a validation set, and a test set,
- try classifiers on the validation set:
  - DecisionTreeClassifier with various max_depth hyperparameter,
  - RandomForestClassifier with various n_estimators and max_depth hyperparameters,
  - LogisticRegression with various solver hyperparameter,
- use the best hyperparameter on the test set,
- make conclusions.

The project was divided into three parts:
- **Profits & Losses:** Identified the biggest profit and loss centers, recommended products to stop selling, found the relationships between total numbers of sales and returns.
- **Advertising:** Identified the best states and months for advertising, calculating the return on ad spend ratio.
- **Returned Items:** Analyzed the return rates of products and examined the relationship between profit and return rates.
