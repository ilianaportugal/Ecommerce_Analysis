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
![alt_text](https://github.com/ilianaportugal/Ecommerce_Analysis/blob/main/Images/Total_OrderAmount_by_Country.png)

Finding(s): Most sales come from the United Kingdom (UK), which is to be expected as the ecommerce store is based in the UK. The Netherlands and Ireland (EIRE), generate the second highest order amounts in terms of sales.

Recommendation(s): Identify any barriers that customers in other countries are facing from purchasing from the store such as shipping costs / expected delivery and try to eliminate these barries by offering free shipping for orders over x amount. 

#### Average Item Quantity per Invoice by Country
![alt_text](https://github.com/ilianaportugal/Ecommerce_Analysis/blob/main/Images/Average_Item_Quantity_by_Country.png)

Finding(s): Netherlands has the highest average item quantity per invoice of 2115, followed by Australia at 1477.

Recommendation(s): The UK average item quantity is on the lower side at 225 items, if we run a promotion that offers a discount at the >250 item mark could significantly increase sales revenue as a majority of customers are based in this location. It would be of interest to identify if the high item order quantity from the Netherlands is from the same customer, as this could be an opportunity to offer a mutually beneficial purchase contract to secure repeat business.

#### Average Order Sum (£) by Country
![alt_text](https://github.com/ilianaportugal/Ecommerce_Analysis/blob/main/Images/Average_Order_Sum_by_Country.png)

Finding(s): This chart follows a similar pattern as the previous "Average Item Quantity per Invoice by Country". The one point that stands out is that Singapor and Lebanon have a significant higher average Order Sum as compared to their average item count, this could be because they are purchasing higher priced items. 

Recommendation(s): The store may consider offering promotions to increase Order sum such as offering free shipping when a total is over X amount. This would incentive customer to spend more and potentially remove a barrier to purchasing.

#### Total Sales (£) by Month
![alt_text](https://github.com/ilianaportugal/Ecommerce_Analysis/blob/main/Images/Total_Sales_by_Month.png)

Finding(s): The store experienced a large spike in Sales in November 2011, they reached just above £14,000,000 in sales that month. This may be because wholesalers are preparing for increased purchasing during the holidays. 

Recommendation(s): Since there is a spike in sales during the holiday months the store should review the items purchased during these times to ensure future inventory can meet demand. The store should also try to capitalize on other holiday celebrations throughout the year such as Valentines by offerring themed items and running marketing/promotions. 

#### Total Orders by Weekday
![alt_text](https://github.com/ilianaportugal/Ecommerce_Analysis/blob/main/Images/Total_Orders_by_Weekday.png)

Finding(s): In this chart we see that most orders are placed on Thursday, Sunday has the lowest number of Orders and no Orders are made on Saturday. It would be interesting to understand if this is because the store doesn't accept Orders, are closed, on Saturday or their customers don't place orders on Satuday. 

Recommendation(s): We should analyze the stores camapigns to understand if there are any email marketing or promotions running on Thursday's that may be contributing to the increase in Orders. If so, these campaigns could be analyzed and tailored to also run on other days of the week. It would also be helpful to identify the reason for zero Orders being placed on Saturdays. If this is because the store is closed they may be missing out on business from companies where Saturday is a working day. 

## Forecasting Model
I created a forecasting model to predict Daily and Monthly sales using Prophet which is a procedure for forecasting time series data based on an additive model. Predicting future sales can be used for planning and goal setting.

#### Actual and Predicted Daily Order Amount (£)

![alt_text](https://github.com/ilianaportugal/Ecommerce_Analysis/blob/main/Images/Actual_and_Predicted_Daily_OrderAmount.png)

#### Actual and Predicted Monthly Order Amount (£)
![alt_text](https://github.com/ilianaportugal/Ecommerce_Analysis/blob/main/Images/Actual_and_Predicted_Monthly_OrderAmount.png)

#### Daily OrderAmount (£) Forecast
![alt_text](https://github.com/ilianaportugal/Ecommerce_Analysis/blob/main/Images/Daily_OrderAmount_Forecast.png)

#### Monthly OrderAmount (£) Forecast 
![alt_text](https://github.com/ilianaportugal/Ecommerce_Analysis/blob/main/Images/Monthly_OrderAmount_Forecast.png)

