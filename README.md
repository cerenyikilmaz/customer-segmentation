# Customer-Segmentation-with-Python
This is my bachelor thesis! I used Python for Customer Segmentation with RFM Analysis. 

-----------------------------------------------------------------------------------------------------------------------------------------------------

This study was created to examine the results to be obtained from the RFM method used in customer segmentation. In this day and age when e-commerce is important, customer loss analysis is one of the sine qua non of this industry. Today's business strategies have prioritized knowing the customer best and determining how to approach the customer. At the same time, data mining, which gives each customer personal access with its features, has become one of the most important tools.
As part of this study, we segmented customers using data from an e-commerce company and analyzed the results.

-----------------------------------------------------------------------------------------------------------------------------------------------------
In our analysis, we used sales data from an e-commerce website for 2021.
We performed our analysis on Jupyter Notebook using Python language. We used the RFM method to segment customers.

-----------------------------------------------------------------------------------------------------------------------------------------------------
We used some libraries in Python to load the dataset, do the analysis and visualize the data. Their names and brief definitions are as follows;

```diff
@@ import pandas @@ 
```
Operations such as reading data, preprocessing, and cleaning are performed with this library.
```diff
@@ import numpy as np @@
```
The Pandas library, which allows us to work with multidimensional arrays and matrices, is also used to perform mathematical operations.
```diff
@@ import datetime as dt @@
```
It's a module that puts at our disposal different functions to work with time, time and date.
```diff
@@ import glob @@
```
It's a module that allows us to list and use specific files in a folder in Python. We used this to import 12 separate CSV files created for 12 months as a single dataframe.
```diff
@@ import os @@
```
It's a module that allows us to work with files and directories with ease.
```diff
@@ from pathlib import Path @@
```
It's a library used to manipulate text files.
```diff
@@ import matplotlib.pyplot as plt @@
```
It's a library that allows us to visualize data through 2 or 3 dimensional drawings.
```diff
@@ import seaborn as sns @@
```
It is a library mainly used for statistical visualizations.
```diff
@@ import squareify @@
```
It is the library that we can use to create treemaps.
```diff
@@ import hashlib @@
```
It is the library used to run various encryption algorithms.

# About Data Set

Our dataset contains sales data from an e-commerce site for 2021. Our dataset contains a total of 6 columns.

customer_id → Identity information unique to each customer making a purchase

item_id → Identity information unique to each product purchased

item_name → Names of purchased items

unit_price → Unit prices of the products

item_count → Number of products purchased

purchase_time → When the customer makes the purchase

In the dataset was defined as the parameters customer_id and unit_price float, item_id and item_count parameters integer, item_name and purchase_time parameters object.

Since we don't need to do any mathematical operations with the customer_id and item_id parameters here, they are used as an object; Since we also need the "purchase_time" parameter as a date, we changed it to "datetime".

Also, because the customer_id parameter comes as an integer, we removed the trailing ".0" values.

Our data set has a total of 16,105,820 rows, 3,706,002 unique item_id and 2,847,919 unique customer_id.

# Brief Description About Segments

Champions: Recently Purchased, Often Purchased, and Most Spent. Reward those customers. You can become an early adopter of new products and help promote your brand.

Loyal Customers: Shop regularly. Responds to promotions.

Potential Loyalist: Recent customers with average frequency. Offer membership or loyalty programs or recommend related products to resell and help them become your loyalists or champions.

New Customers: Purchased recently, but not often. Start building relationships with these customers by offering onboarding support and special offers to increase their visits.

Promising: New buyers but not much spent.

Need Attention: Above-average topicality, frequency and monetary values. I may have bought it recently though.

About to Sleep: below-average timeliness and frequency. Lose them if they don't reactivate.

At Risk: Some time since purchase. I have to bring her back! Send them personalized reactivation campaigns to reconnect and offer renewals and helpful products to encourage another purchase.

Can't Lose: Often bought in the past, but haven't returned it for a long time. Bring them back with relevant promotions and conduct surveys to find out what went wrong and avoid losing them to a competitor.

Hibernating: Last purchase was a long time ago and low number of orders. Can be lost.

# Comparison of Results and Recommendations

Below we see the results of the segments as a result of the two requests we made by dividing them into 4 clusters and 5 clusters.
segments with a conspicuously high difference between them; At Risk, Hibernating, New Customers, Potential Loyalists and Promising.

The At Risk and Hibernating segments include clients that I have lost or are about to lose. While their number is low when I use 4 clusters, if we narrow down the results and break them into 5 clusters, we see that they are quite high. In this context, it would be more logical to examine the customers in 5 clusters instead of 4 clusters. That way, more solid steps can be taken to minimize customer loss.

![Alt text](/compare.png?raw=true "Optional Title")

We should try to reconnect with customers in the About to Sleep segment. We can win them back by offering special discounts, popular offers and sharing our valuable resources with them.

In order to reconnect customers in “At Risk”, we may try to bring them back by sending them personalized emails or other personalized messages.

The Can't Lose customer segment is one of the segments that should be given importance. These are the customers we don't want to lose. This group has not been shopping for a long time, but the total number of purchases is quite high. We can conduct surveys and get their opinions to find out what went wrong in that segment. We should also offer campaigns that make these customers feel valued.

Focusing on satisfying customers in the Champions, Loyal Customers, Potential Loyalists, and Promising segments should be a priority. It will be a plus to reach them in a more personalized way, by analyzing their individual preferences and affinities more. For example, personal messages such as birthday wishes can be sent. New promotions for products can be reported early.

People in the Need Attention segment are the customer group we tend to lose by showing averages both in time and in terms of total purchases, while at the same time it doesn't take much effort to win. We may make limited time offers in this segment that will entice them to shop with us. We can recommend products based on previous purchases. This way we can reactivate them so that they can shop.

The customer group New Customers are groups who recently had new contacts. We need to increase the overall purchases of this segment. We should have them come to us often, even for small sums. We can organize special promotions for new customers.
