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
  - https://medium.com/analytics-vidhya/how-to-determine-the-optimal-k-for-k-means-708505d204eb
  
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
# Model Builiding

## K-means

The K-Means is an unsupervised machine learning algorithm. It works by grouping data points with similar attribute values together by measuring the euclidean distances between them. It is simple and perhaps the most commonly used algorithm for clustering.

The basic idea behind k-means consists of defining k clusters such that total within-cluster variation (or error) is minimum.

Two methods that can be useful to find this mysterious k in k-Means are:
- The Elbow Method
- The Silhouette Method

### The Elbow Method

Calculate the Within-Cluster-Sum of Squared Errors (WSS) for different values of k, and choose the k for which WSS becomes first starts to diminish. In the plot of WSS-versus-k, this is visible as an elbow.

Within-Cluster-Sum of Squared Errors sounds a bit complex. Let’s break it down:

- The Squared Error for each point is the square of the distance of the point from its representation i.e. its predicted cluster center.
- The WSS score is the sum of these Squared Errors for all the points.
- Any distance metric like the Euclidean Distance or the Manhattan Distance can be used

### The Silhouette Method

The silhouette value measures how similar a point is to its own cluster (cohesion) compared to other clusters (separation).

The range of the Silhouette value is between +1 and -1. A high value is desirable and indicates that the point is placed in the correct cluster. If many points have a negative Silhouette value, it may indicate that we have created too many or too few clusters.

The Silhouette Score reaches its global maximum at the optimal k.

---
# Dimesionality Reduction

## Autoencoders

Autoencoder is an unsupervised artificial neural network that learns how to efficiently compress and encode data then learns how to reconstruct the data back from the reduced encoded representation to a representation that is as close to the original input as possible.

Autoencoder, by design, reduces data dimensions by learning how to ignore the noise in the data.




