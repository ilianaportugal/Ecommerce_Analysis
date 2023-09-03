# Ecommerce_Analysis
## Purpose
The purpose of this project is to analyze an ecommerce dataset to identify trends and propose recommendations to increase sales. In this project I also trained a time series forecasting model to predict future sales based on historical values for Daily and Monthly order amounts.

## Overview

#### Analysis:
[ecommerce_analysis.ipynb](https://github.com/ilianaportugal/Ecommerce_Analysis/blob/main/ecommerce_analysis.ipynb)

#### Dataset:
[ecommerce_dataset.csv](https://github.com/ilianaportugal/Ecommerce_Analysis/blob/main/DataSource/ecommerce_dataset.csv)

#### About the Dataset: 
This is a transnational data set which contains all the transactions occurring between 12/01/2010 and 12/09/2011 for a UK-based and registered non-store online retail. The company mainly sells unique all-occasion gifts. Many customers of the company are wholesalers.

#### Columns:
InvoiceNo, StockCode, Description, Quantity, InvoiceDate, UnitPrice, CustomerID, Country

#### Environment:
Jupyter Notebook

#### Languages:
Python

#### Dependencies:
Pandas, Matplotlib, Sktime

## Objectives
(1) Perform exploratory analysis by creating dataframes and calculated fields

(2) Create visualizations to show relationships and identify trends

(3) Create a Forecast Model with Prophet that predicts known sales

(4) Create a Forecast Model with Prophet that predicts future sales 

## Data Visualizations and Results
#### Total Order Amount (£) by Country
![alt_text](https://github.com/ilianaportugal/Ecommerce_Analysis/blob/949f689c1484ec24f3e5bba76f3c9733d91731b7/Images/Total_Order_Amount_by_Country.png)

Finding(s): Most sales come from the United Kingdom (UK), which is to be expected as the ecommerce store is based in the UK. The Netherlands and Ireland (EIRE), generate the second highest amount in terms of sales.

Recommendation(s): Identify any barriers that customers in other countries are facing from purchasing from the store such as shipping costs / expected delivery and try to eliminate these barries by offering free shipping for order over x amount. 

#### Total Orders by Country
![alt_text](https://github.com/ilianaportugal/Ecommerce_Analysis/blob/949f689c1484ec24f3e5bba76f3c9733d91731b7/Images/Total_Orders_by_Country.png)

Finding(s):

Recommendation(s):

#### Average Item Quantity per Invoice by Country
![alt_text](https://github.com/ilianaportugal/Ecommerce_Analysis/blob/949f689c1484ec24f3e5bba76f3c9733d91731b7/Images/Average_Item_Quantity_by_Country.png)

Finding(s): Netherlands has the highest average item quantity per invoice of 1981, followed by Australia at 1212.

Recommendation(s): The UK average item quantity is on the lower side at 181 items, if we run a promotion that offers a discount at the >200 item mark could significantly increase sales revenue as a majority of customers are based in this location. It would be of interest to identify if the high item order quantity from the Netherlands is from a repeat customer, as this could be an opportunity to offer a mutually beneficial purchase contract. 

#### Average Order Sum (£) by Country
![alt_text](https://github.com/ilianaportugal/Ecommerce_Analysis/blob/949f689c1484ec24f3e5bba76f3c9733d91731b7/Images/Avergage%20Order%20Sum%20by%20Country.png)

Finding(s): This chart follows a similar pattern as the previous one "Average Item Quantity per Invoice by Country". The one point that stands out is that Lebanon has a significant higher average Order Sum as compared to their average item count, this could be because they are purchasing higher priced items. 

Recommendation(s):

#### Total Sales (£) by Month
![alt_text](https://github.com/ilianaportugal/Ecommerce_Analysis/blob/949f689c1484ec24f3e5bba76f3c9733d91731b7/Images/Total%20Sales%20by%20Month.png)

Finding(s): The store experienced a large spike in Sales in 10/2011 and 11/2011 where they reached just above £14,000,000 in sales that month. This is expected as wholesalers are most likely preparing for increased purchasing during the holidays. Between 12/2010 and 08/2011 sales are slightly below £8,000,000.

Recommendation(s): Since there is a spike in sales during the holiday months the store should review the items purchased during these times to ensure future inventory can meet demand.

#### Total Orders by Weekday
![alt_text](https://github.com/ilianaportugal/Ecommerce_Analysis/blob/949f689c1484ec24f3e5bba76f3c9733d91731b7/Images/Total%20Orders%20by%20Weekday.png)

Finding(s):

Recommendation(s):

## Forecasting Model
The dataset included sales data between the dates 12/1/2010 and 12/9/2011. I created a forecasting model to predict Daily and Monthly sales using Prophet which is a procedure for forecasting time series data based on an additive model. Predicting future sales can be used for planning and goal setting.
