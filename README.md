# Ecommerce_Analysis
## Purpose
The purpose of this project is to analyze an ecommerce dataset to identify trends and propose recommendations to increase sales. In this project I also trained a time series forecasting model to predict future sales based on historical values for Daily and Monthly order amounts.

## Overview

#### Analysis:
[ecommerce_analysis.ipynb](https://github.com/ilianaportugal/Ecommerce_Analysis/blob/main/ecommerce_analysis.ipynb)

#### Dataset:
[ecommerce_dataset.csv](https://github.com/ilianaportugal/Ecommerce_Analysis/blob/main/DataSource/ecommerce_dataset.csv)

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

(2) Create charts to show relationships and identify trends

(3) Create a Forecast Model with Prophet that predicts known sales

(4) Create a Forecast Model with Prophet that predicts future sales 

## Data Visualizations and Results
#### Total Order Amount ($) by Country
![alt_text](https://github.com/ilianaportugal/Ecommerce_Analysis/blob/949f689c1484ec24f3e5bba76f3c9733d91731b7/Images/Total_Order_Amount_by_Country.png)

#### Total Orders by Country
![alt_text](https://github.com/ilianaportugal/Ecommerce_Analysis/blob/949f689c1484ec24f3e5bba76f3c9733d91731b7/Images/Total_Orders_by_Country.png)

#### Average Item Quantity by Country
![alt_text](https://github.com/ilianaportugal/Ecommerce_Analysis/blob/949f689c1484ec24f3e5bba76f3c9733d91731b7/Images/Average_Item_Quantity_by_Country.png)

#### Average Order Sum ($) by Country
![alt_text](https://github.com/ilianaportugal/Ecommerce_Analysis/blob/949f689c1484ec24f3e5bba76f3c9733d91731b7/Images/Avergage%20Order%20Sum%20by%20Country.png)

#### Total Sales ($) by Month
![alt_text](https://github.com/ilianaportugal/Ecommerce_Analysis/blob/949f689c1484ec24f3e5bba76f3c9733d91731b7/Images/Total%20Sales%20by%20Month.png)

#### Total Orders by Weekday
![alt_text](https://github.com/ilianaportugal/Ecommerce_Analysis/blob/949f689c1484ec24f3e5bba76f3c9733d91731b7/Images/Total%20Orders%20by%20Weekday.png)

## Forecasting Model
The dataset included sales data between the dates 12/1/2010 and 12/9/2011. I created a forecasting model to predict Daily and Monthly sales using Prophet which is a procedure for forecasting time series data based on an additive model. Predicting future sales can be used for planning and goal setting.
