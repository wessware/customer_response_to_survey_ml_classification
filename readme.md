# Problem Statement

In this Data science project, the intention is create a model that can help a company identify the most suitable customers to include in a current campaign based on the customer's historical data in dealing with the company.

Since the company has thousands of customers who might have used their services in the past, it is easily possible to tell which customers would be [still] be interested in new products launched by the company.

## The Data

Each row of this set relates to a customer's interactions during one marketing campaign "this campaign".
This is historical data, so for each one we know whether the customer ended up taking out a new contract
(that is, responded positively to the campaign). Each customer may also have been reached by a previous marketing campaign, and if so then the details of that contact are recorded under the features with "previous_campaign" in their name.

## Input variables

ID: unique identifier for this record
town: home town for customer
country: country for customer's home address
age: customer's age
job: customer's job
married: customer's marital status
education: customer's highest educational qualification level obtained
arrears?: has the customer failed to pay a recent bill?
current_balance: current amount in customer's landline account in pounds (could be negative)
housing: is the customer a homeowner?
has_tv_package: has the customer got an additional TV and data package on their landline
last_contact: type of communication used for previous call to customer
conn_tr: connection type grouping ID (related to the connection for their landline)
last_contact_this_campaign_month: last contact month of year
last_contact_this_campaign_day: last contact day of the month
this_campaign: number of contacts performed during this campaign and for this client
days_since_last_contact_previous_campaign: number of days that passed by after the client was last contacted from a previous campaign
(-1 means the client has never been contacted before)
contacted_during_previous_campaign: number of contacts performed before this campaign and for this client
outcome_previous_campaign: outcome of the previous marketing campaign

The Target Variable
new_contract_this_campaign: has the client taken out a new contract?

## Modelling

The best method to model and predict outcomes for this kind of problem was seen to be classification. However, other approaches such as linear regression and clustering can still be used to fit and train the machine learning model on this problem.
Classification and regression models were fitted in order to determine the best performing models for each approach.
An Artificial Nueral Network classification model was as well fitted and trained on the data.

## Classifiers

1. Ensemble tree-based machine learning classifier - Random Forest
2. Artificial Neural Networks classifier

## Regressors

1. Linear regressor
2. Random Forest Regressor
3. Xtreme Gradient Boosting Regressor.

## Tuning and Evaluation

Each fitted and trained model was tuned using different parameters and hyperparameters in so to give the score possible.

### Evaluation Metrics

### rmse [best performing to least performing]

1. Random Forest Regressor [rmse - 0.1]
2. XGB Regressor [rmse - 0.13]
3. Artificial Neural Network [rmse - 0.3]

### Confusion Matrix

1. Random Forests Classifier
Accuracy - 82%
