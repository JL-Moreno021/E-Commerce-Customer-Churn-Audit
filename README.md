# Project Overview
## [E-Commerce Customer Churn Audit](https://www.kaggle.com/datasets/waddahali/e-commerce-customer-churn-audit?select=customer+churn.csv)
    - Synthetix E-Commerce: Behavioral Churn Dataset<br>
    - This dataset represents a simulated e-commerce environment designed to challenge data scientists in the areas of data cleaning, exploratory data analysis (EDA), and predictive modeling. It contains a mix of demographic, behavioral, and transactional data for 10,300 customers.

**_Note:_** This dataset represents a simulated e-commerce environment designed to challenge data scientists in the areas of data cleaning, exploratory data analysis (EDA), and predictive modeling. It contains a mix of demographic, behavioral, and transactional data for 10,300 customers.
<br>
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
>>---

#### **_Numeric Data Types_**<br>
>- Use describe() to view invalid observations
    - Invalid numeric values
    - Duplicate values on unique field

>>>---

#### **_Findings_**
>>>---
> **_Age_**<br>
    - have min value of `-10`
    - have big outlier
<br>

> **_Customer Service Calls_**<br>
    - have min value of `-1`
<br>

> **_Monthly Spend_**<br>
    - have min value of `-10`
    - have big outlier
>>>---
#### **_Process_**<br>
>>---
Convert all non-positive values in `Age`, `Customer Service Calls`, and `Monthly Spend` into `nan`

> **_Age Outlier_**<br>
    - Check for the second highest age

> **_Process_**<br>
    - Use the second highest age as the maximum age
    - nullify outlier age (can be an error)

> **_Monthly Spend Outlier_**<br>
    - Check for the second highest monthly spending value

> **_Process_**<br>
    - Use the second highest monthly spending value as the maximum value
    - nullify outliers (can be an error)

<hr>

#### **_String Data Types_**<br>
>- Use `set()` to view unique observations and to identify typographical errors
    - Duplicate
    - Typographical Errors
<hr>

>>>---

#### **_Findings_**
>>>---
> **_Region_**<br>
    - Some values are not capitalized and is a duplicate
<br>

> **_Subscription Plan_**<br>
    - have min value of `-1`
>>>---
#### **_Process_**<br>
>>---
Convert all `Region` and `Subscription Plan` to _Capitalized_ format