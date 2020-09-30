# Credit-Card-Customer-Segmentation

---
# Project Overview

- Objective : **To do Customer Segmentation on Credit Card Data** 
- Clustering Model
- Data cleaning and Data preprocessing
- Exploratory Data Analysis
- **K-means Clustering**
- **PCA** used for Model Visualization
- **Autoencoders Model** used for Dimensionality Reduction to improve Cluster Analysis

---
# About Project

We are doing customer segmentation on credit card customer dataset so that we can analyse their customers and identify their needs.

As we know, marketing is very important for growth and development of any company. By using customer segmentation, they can target specific customers according to their need which helps the company to increase their sales and revenue.

---
# Code and Resources used

- Python version: 3.7.6
- Packages: Pandas, Numpy, Seaborn, Matplotlib, Scikit, Tensorflow and Keras
- Resources used:

---
# Web Scraping

Dataset URL: https://www.kaggle.com/arjunbhasin2013/ccdata 

The sample Dataset summarizes the usage behavior of about 9000 active credit card holders during the last 6 months. The file is at a customer level with 18 behavioral variables.
Following is the Data Dictionary for Credit Card dataset :-

- CUSTID : Identification of Credit Card holder (Categorical)
- BALANCE : Balance amount left in their account to make purchases (
- BALANCEFREQUENCY : How frequently the Balance is updated, score between 0 and 1 (1 = frequently updated, 0 = not frequently updated)
- PURCHASES : Amount of purchases made from account
- ONEOFFPURCHASES : Maximum purchase amount done in one-go
- INSTALLMENTSPURCHASES : Amount of purchase done in installment
- CASHADVANCE : Cash in advance given by the user
- PURCHASESFREQUENCY : How frequently the Purchases are being made, score between 0 and 1 (1 = frequently purchased, 0 = not frequently purchased)
- ONEOFFPURCHASESFREQUENCY : How frequently Purchases are happening in one-go (1 = frequently purchased, 0 = not frequently purchased)
- PURCHASESINSTALLMENTSFREQUENCY : How frequently purchases in installments are being done (1 = frequently done, 0 = not frequently done)
- CASHADVANCEFREQUENCY : How frequently the cash in advance being paid
- CASHADVANCETRX : Number of Transactions made with "Cash in Advanced"
- PURCHASESTRX : Numbe of purchase transactions made
- CREDITLIMIT : Limit of Credit Card for user
- PAYMENTS : Amount of Payment done by user
- MINIMUM_PAYMENTS : Minimum amount of payments made by user
- PRCFULLPAYMENT : Percent of full payment paid by user
- TENURE : Tenure of credit card service for user

---
# Data Cleaning

I made the following changes and created the following variables:

- Set NULL values for “minimum payments” and “credit limit” with mean data
- Remove column “customer ID”

---
# EDA

I looked at the distributions of the data and the value counts for the various numerical variables. Below are a few highlights:

![](https://github.com/SidSolanki28/Credit-Card-Customer-Segmentation/blob/master/Images/index.png)

---




