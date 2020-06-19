# Bank Marketing Project
Predictive modelling to optimize marketing campaign for Portuguese bank client

## Executive Summary
The client can optimize conversion in its marketing campaign by planning multiple attempts per customer, targeting younger customers with greater needs for incremental credit.

## Goal of Project
The goal of this project was to provide 
1)  Actionable insights on drivers that contributed to campaign conversion to be employed in subsequent campaigns
2)  A predictive model, ensemble or otherwise, to predict conversion in this and future campaigns (assuming same inputs are available and used)

## Data, Assumptions, & Methodology

### Data
The data used was provided by the client via the UC Irvine data science repository (Link). There were XX observations with no missing data in the provided observations.

### Assumptions
It was assumed that this data are either comprehensive to the marketing campaign or a representative sample of the campaign as a whole.

### Methodology
The provided data was split into train and test sets using an 80/20 split to train predictive models and test the performance of those models, respecitvely. Models were trained and optimized using a fixed cross-validation method, which used the same 10-fold cross-validation indices to train each model. This was to ensure comparison of model performance was truly "apples to apples," as each model was trained on exactly the same data. <br />

Further, multiple models were trained for each method using hyperparameter tuning (where appropriate) to enhance model predictive performance. All data processing, model training, etc. was conducted in the R Studio IDE. <br />

<b>Predictive models used include:</b> <br />
Model Type (<em>method</em>)  <br />
Multi-variate Generalized Linear Model (<em>glm</em>)  <br />
CART Decision Tree (<em>rpart</em>)  <br />
Random Forest (<em>ranger</em>)  <br />
Ridge and Lasso Regression Model (<em>glmnet</em>)  <br />
Gradient Boosted Tree (<em>xgboost</em>)  <br />
