# Customer Churn Analysis

## Introduction

- In today's competitive business environment, retaining customers is crucial for long-term success. Churn analysis is a key technique used to understand and reduce this customer attrition.
- This is a Power BI and SQL project on churn analysis of an imaginary telecommunication company. This project is to examine customer data to identify patterns and reasons behind customer departures. And use advanced data analytics and machine learning, to predict which customers are at risk of leaving and understand the factors driving their decisions.
---
![](churn7.png)
---
## Problem Statement
1. Are there specific demographic segments like age and gender, that are more likely to churn?
2. Are there regional variations in churn rates?
3. Which services or bundles are associated with higher churn rates?
4. Can we develop a predictive model to identify customers at risk of churning before they leave?

## Data Sourcing

The Customer Data csv file contains 6418 rows with 32 columns

## Data Transformation
### Data Cleaning:

- Handling Null Values: The code uses the ISNULL function to replace null values with default values like "None" or "No" for certain columns. This ensures data consistency and avoids errors during analysis.

Identifying Null Values                        |          Removing Null Values
:---------------------------------------------:|:------------------------------------:
  ![](Null_values.jpg)                         |            ![](remove_null.jpg)
  
### Data Type Conversion: 
- The code potentially converts the Bit data type to Varchar(50) to address compatibility issues with the Import Wizard.

### Data Validation:
- The code likely sets a primary key (CustomerID) to prevent duplicate entries in the data.

### Data Exploration:
- The code uses SELECT, COUNT, and GROUP BY to explore the data and understand its characteristics.
- This includes counting distinct values, checking for nulls, and calculating summary statistics.

## Skills Demonstrated

The following SQL features were incorporated;
- Query Writing
- Data Modification; This includes INSERT, UPDATE, DELETE
- Filtering and Sorting
- Aggregation
- Subqueries
- Indexing
- Views
- Transactions

The following Power BI features were incorporated;
- DAX
- Quick Measures
- Page Navigation
- Filters
- Tooltips
- Button





## Project Target

Create an entire ETL process in a database & a Power BI dashboard to utilize the Customer Data and achieve below goals:
        
    Visualize & Analyse Customer Data at below levels
    Demographic
    Geographic
    Payment & Account Info
    Services
    Study Churner Profile & Identify Areas for Implementing Marketing Campaigns
    Identify a Method to Predict Future Churners
 

Metrics Required

    Total Customers
    Total Churn & Churn Rate
    New Joiners

### Churn Analysis Summary Dashboard
![Churn_Analysis_Summary_Dashboard](https://github.com/user-attachments/assets/4cde275e-3490-4076-bd28-266c62e51ff4)

## Predict Customer Churn

For predicting customer churn, used Machine Learning algorithm called RANDOM FOREST.

### What is Random Forest?
A random forest is a machine learning algorithm that consists of multiple decision trees. Each decision tree is trained on a random subset of the data and features. The final prediction is made by averaging the predictions (in regression tasks) or taking the majority vote (in classification tasks) from all the trees in the forest. This ensemble approach improves the accuracy and robustness of the model by reducing the risk of overfitting compared to using a single decision tree.

### Churn Prediction Dashboard
![Churn_Prediction_Dashboard](https://github.com/user-attachments/assets/10d4500f-5cae-43f5-9fbc-82f92dcd9eea)
