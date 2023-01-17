# Cohort-Analysis---Retail-store
## Problem Statement
We have to perform cohort and RFM analysis to understand the value derived from different customer segments. Further, we will divide customers in different clusters based on the analysis by using K-means algorithm.

## Dataset Description
This is a transactional data set which contains all the transactions that occurred between 01/12/2010 and 09/12/2011 for a UK-based and registered non-store online retail. The company mainly sells unique and all-occasion gifts.

### Variables	Description
- **InvoiceNo**	Invoice number. Nominal, a six digit integral number uniquely assigned to each transaction. If this code starts with letter 'c', it indicates a cancellation
- **StockCode**	Product (item) code. Nominal, a five digit integral number uniquely assigned to each distinct product
- **Description**	Product (item) name. Nominal
- **Quantity**	The quantities of each product (item) per transaction. Numeric
- **InvoiceDate**	Invoice Date and time. Numeric, the day and time when each transaction was generated
- **UnitPrice**	Unit price. Numeric, product price per unit in sterling
- **CustomerID**	Customer number. Nominal, a six digit integral number uniquely assigned to each customer
- **Country**	Country name. Nominal, the name of the country where each customer resides

## Retention Analysis :  
Retention analysis allows you to understand customer behavior when it comes to using and abandoning your product so you can maintain healthy growth through constantly improving retention.   

Perform a retention analysis using:  

* Cohort analysis to detect which user cohort churns the most over a defined period (usually a year).   
* Funnel analysis to understand steps in the customer journey that gets users to drop off.   
* A customer engagement score will help you anticipate churn by tracking users’ activity and signalling when they become disengaged.   

## Cohort Analysis

A cohort is a group of subjects who share a defining characteristic. We can observe how a cohort behaves across time and compare it to other cohorts. 

#### Types of cohorts:

- **Time Cohorts** are customers who signed up for a product or service during a particular time frame. Analyzing these cohorts shows the customers’ behavior depending on the time they started using the company’s products or services. The time may be monthly or quarterly even daily.
- **Behavior cohorts** are customers who purchased a product or subscribed to a service in the past. It groups customers by the type of product or service they signed up. Customers who signed up for basic level services might have different needs than those who signed up for advanced services. Understaning the needs of the various cohorts can help a company design custom-made services or products for particular segments.
- **Size cohorts** refer to the various sizes of customers who purchase company’s products or services. This categorization can be based on the amount of spending in some periodic time after acquisition or the product type that the customer spent most of their order amount in some period of time.

***For cohort analysis, there are a few labels that we have to create:***

- **Invoice period** - A string representation of the year and month of a single transaction/invoice.
- **Cohort group:**- A string representation of the the year and month of a customer’s first purchase. This label is common across all invoices for a particular customer.
- **Cohort period/Index**-  A integer representation a customer’s stage in its “lifetime”. The number represents the number of months passed since the first purchase.
