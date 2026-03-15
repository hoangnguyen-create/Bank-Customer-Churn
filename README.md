# Bank Customer Churn
The primary objective of this project is to identify the main factors that drive customers to churn and to develop a predictive model capable of estimating churn probability at the individual customer level.

By understanding churn drivers and predicting high-risk customers, the bank can develop loyalty programs and retention strategies to improve customer lifetime value and reduce revenue loss.

### Research question: 
1. What key demographic, behavioral, and financial factors significantly influence customer churn in the bank?

2. How do customer engagement indicators (ex: active membership, product usage, complaints, satisfaction score) relate to churn behavior?

3. Can we build a predictive model to estimate the probability of customer churn and identify high-risk customers for targeted retention strategies?

### Expected outcomes:

* Identification of statistically significant churn drivers

* Quantification of impact for each key variable

* Development of a machine learning model to predict churn probability

* Actionable business recommendations to improve retention

### Dataset: Bank Customer Churn

Dataset URL: https://www.kaggle.com/datasets/radheshyamkollipara/bank-customer-churn

### Dataset structure:

The dataset contains **10,000 bank customers** with demographic, financial, and behavioral attributes.

**Key variables** include:

**CreditScore** – Customer credit score

**Geography** - Location of customer

**Gender** - Gender of customer

**Age** – Customer age

**Tenure** – Number of years the customer has stayed with the bank

**Balance** – Account balance

**NumOfProducts** – Number of banking products owned

**HasCrCard** – Whether the customer owns a credit card

**IsActiveMember** – Whether the customer is actively using banking services

**EstimatedSalary** – Estimated annual salary

**Exited** – Target variable indicating whether the customer churned

**Complaint** - Whether the customer makes a complaint

**Satisfaction Score** - Score provided by the customer for their complaint resolution.

**Card Type** - Type of card held by the customer.

**Points Earned** - The points earned by the customer for using a credit card.

Some identifier columns such as **RowNumber**, **CustomerId**, and **Surname** were removed during data cleaning because they do not provide meaningful predictive information as well as to ensuring customer's privacy

## Project Workflow

The analysis follows a typical data analytics pipeline:

**1. Data Cleaning**

* Removed identifier variables

* Checked for missing values

* Verified data types

**2. Exploratory Data Analysis**

* Summary statistics

* Correlation heatmap

* Distribution analysis

* Boxplot analysis for key variables

**3. Feature Selection**

* Selected key variables based on correlation analysis and business relevance

**4. Logistic Regression Modeling**

* Built a logistic regression model to estimate the probability of customer churn

**5. Model Evaluation**

* Interpreted model coefficients

* Analyzed statistical significance
