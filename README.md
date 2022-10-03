# Amazon_Vine_Analysis
Module 16

## Overview
*Background and Purpose*

Since the work with Jennifer on the SellBy project was successful, another, larger project has been assigned. Now we will be analyzing Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

This project will utilize approximately 50 datasets. Each one contains reviews of a specific product, from clothing apparel to wireless products. One of the datasets will be chosen, and PySpark will be used to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, PySpark, Pandas, or SQL will be used to determin potential bias toward favorable reviews from Vine members in the dataset. Then, a summary will contain the analysis for Jennifer to submit to the SellBy stakeholders.

## Software

- Google Colab
- Spark—PySpark 
- Amazon Web Services (AWS)
  - Relational Database Service (RDS)—PostgreSQL 
- pgAdmin 4

## Deliverable 1: Perform ETL on Amazon Product Reviews

[Successful Linkage between AWS and PgAdmin - Customer Table](https://github.com/nadiezhdamhb/Amazon_Vine_Analysis/blob/main/Images/customers_table.png)

![Customer Table](https://github.com/nadiezhdamhb/Amazon_Vine_Analysis/blob/main/Images/customers_table.png)

![Customer Table](https://github.com/nadiezhdamhb/Amazon_Vine_Analysis/blob/main/Images/customers_table.png)







## Summary

*Bias: Not Present*

Based on the results above, there was no bias present within the Vine program. The non-Vine Reviews (unpaid reviews) are in higher quality and there are more with a 5-star rating. The results do not show that Vine is doing significantly better than non-Vine, so I would not conclude on any bias being apparent, at this level of analysis.

*Additional Analysis*

In the future, more analyses should be run to possibly filter other columns of the dataset that might lead to a better understanding of the data. The verified purchase column would be helpful to perform this on because by comparing the ratings on verified purchases for both paid and unpaid reviews. It would also be helpful to more carefully track which users are leaving the most reviews. This could help to verify that the reviews are "real" and that the reviewer actually bought the product.

A useful filter would also be to search through the reviews and determine how rating differ from each other. If the paid reviews (Vine reviews) were higher on similar products, then there might be a possiblity of bias present.
