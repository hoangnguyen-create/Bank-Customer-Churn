# Bank Customer Churn
The primary objective of this project is to identify the main factors that drive customers to churn and to develop a predictive model capable of estimating churn probability at the individual customer level.

By understanding churn drivers and predicting high-risk customers, the bank can develop loyalty programs and retention strategies to improve customer lifetime value and reduce revenue loss.

### Research question: 
What key demographic, behavioral, and financial factors significantly influence customer churn in the bank?
How do customer engagement indicators (ex: active membership, product usage, complaints, satisfaction score) relate to churn behavior?
Can we build a predictive model to estimate the probability of customer churn and identify high-risk customers for targeted retention strategies?

### Expected outcomes:

Identification of statistically significant churn drivers
Quantification of impact for each key variable
Development of a machine learning model to predict churn probability
Actionable business recommendations to improve retention

### Dataset: Bank Customer Churn

Dataset URL: https://www.kaggle.com/datasets/radheshyamkollipara/bank-customer-churn

### Dataset structure:

RowNumber - corresponds to the record (row) number 

CustomerId - unique identifier for customers 

Surname - the surname of customer

CreditScore - can have an effect on customer churn, since a customer with a higher credit score is less likely to leave the bank

Geography - a customer’s location can affect their decision to leave the bank

Gender - gender of customer

Age - customer’s age 

Tenure - number of years that the customer has been a client of the bank. 

Balance - bank balance of a customer

NumOfProducts - number of products that a customer has purchased through the bank.

HasCrCard - denotes whether or not a customer has a credit card

IsActiveMember—active customers are less likely to leave the bank.

EstimatedSalary - customer’s salary 

Exited - whether or not the customer left the bank.

Complaint - customer has complaint or not.

Satisfaction Score - Score provided by the customer for their complaint resolution.

Card Type - type of card held by the customer.

Points Earned - the points earned by the customer for using a credit card.

### Initial Analysis plan:

Data cleaning: Handled missing value, correct data types and remove duplicate 

EDA: Explore dataset structure, detect patterns, analyze distributions, and evaluate relationships between features and churn

Analysis: Identify key churn drivers using statistical analysis and feature correlation

Visualization: Create histograms,  correlation heatmaps, and prediction model to generate actionable insights

Data Storytelling: present findings and relationship between variables that affect customer churning as well as recommending retention strategy to enhance customers’ loyalty 
