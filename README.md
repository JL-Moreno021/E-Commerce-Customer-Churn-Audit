# Project Overview
## [E-Commerce Customer Churn Audit](https://www.kaggle.com/datasets/waddahali/e-commerce-customer-churn-audit?select=customer+churn.csv)
    - Synthetix E-Commerce: Behavioral Churn Dataset<br>
    - This dataset represents a simulated e-commerce environment designed to challenge data scientists in the areas of data cleaning, exploratory data analysis (EDA), and predictive modeling. It contains a mix of demographic, behavioral, and transactional data for 10,300 customers.

<div class='alert alert-block alert-warning'><b>This dataset was synthetically generated and may not reflect real-world data.<b></div>

**_Publisher:_** [Waddah Ali](https://www.kaggle.com/waddahali)

## Dataset Overview

### Evironment Setup and Packages

#### **_Package Manager_**
    - UV

#### **_Packages_**
    - pandas
    - jupyter

#### **_Language_**
    - python 3.14.6

### Dataset Summary Findings
> _Payment Method_ and _Age_ have null values

## Data Cleaning Overview

### Data Observations Checking
<hr>

**_Numeric Data Types_**<br>
    - Use describe() to view invalid observations
>- Invalid numeric values
>- Duplicate values on unique field
>>---
> **_Findings_**
>>---
>> **_Age_**
>>>- have min value of `-10`
>>>- have big outlier
<br>

>> **_Customer Service Calls_**
>>>- have min value of `-1`
<br>

>> **_Monthly Spend_**
>>>- have min value of `-10`
>>>- have big outlier
<hr>