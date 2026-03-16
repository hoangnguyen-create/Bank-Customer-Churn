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

### Tools Used

* Python

* Pandas

* NumPy

* Seaborn

* Matplotlib

* Statsmodels

* Power BI

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

### Explaratory Data Analysis

![image alt](https://github.com/hoangnguyen-create/Bank-Customer-Churn/blob/6647c06a155e01218488c121e86b3f1a6682b6e1/Images/DF%20-%20HEAD.png)

![image alt](https://github.com/hoangnguyen-create/Bank-Customer-Churn/blob/6647c06a155e01218488c121e86b3f1a6682b6e1/Images/DF%20-%20INFO.png)

![image alt](https://github.com/hoangnguyen-create/Bank-Customer-Churn/blob/6647c06a155e01218488c121e86b3f1a6682b6e1/Images/POWER%20BI%20DASHBOARD.png)

![image alt](https://github.com/hoangnguyen-create/Bank-Customer-Churn/blob/6647c06a155e01218488c121e86b3f1a6682b6e1/Images/DF%20-%20EXITED%20VALUE%20COUNT.png)

Almost all churned customers filed complaints. Approximately **99.8%** of churned customers had previously complained, indicating that the variable "Complain" occurs very close to the churn event and may introduce data leakage in the model. The variable "Complain" was therefore excluded from modeling. 

![image alt](https://github.com/hoangnguyen-create/Bank-Customer-Churn/blob/6647c06a155e01218488c121e86b3f1a6682b6e1/Images/CORRELATION%20HEATMAP.png)


EDA revealed several patterns related to customer churn:

* **Age** shows a weak positive correlation with customer churn (0.29), indicating that older customers are more likely to leave the bank

* Customers with **higher account balances** tend to have a higher probability of churn.

* **Active members** are significantly less likely to churn compared to inactive customers.

* The correlation heatmap also showed that **some variables** have weak relationships with churn and were therefore **excluded** from the final model.

Additionally, a boxplot analysis of **Age vs Churn** further confirmed that churned customers tend to be older than those who remain with the bank.

![image alt](https://github.com/hoangnguyen-create/Bank-Customer-Churn/blob/6647c06a155e01218488c121e86b3f1a6682b6e1/Images/BOXPLOT.png)

### Logistic Regression Model

A logistic regression model was developed using the following variables:

1. Age

2. Balance

3. IsActiveMember

![image alt](https://github.com/hoangnguyen-create/Bank-Customer-Churn/blob/6647c06a155e01218488c121e86b3f1a6682b6e1/Images/LOGISTIC%20REGRESSION%20MODEL.png)

The model results show that all selected variables are statistically significant predictors of customer churn (LLR p-value < 0.05).

Key findings from the model:

* Age has a positive relationship with churn probability.

* Higher balances slightly increase the likelihood of churn.

* Active membership significantly reduces the probability of customer churn.

## Business Recommendations 

Based on the analysis, the following strategies are recommended:

1. Focus on develop **targeted retention campaigns** for older customers.

2. Offer **personalized financial incentives** for high-balance customers to reduce churn risk.

3. Strengthen customer **engagement programs** or advertise **exclusive member benefits** to encourage inactive customers to become active users.

