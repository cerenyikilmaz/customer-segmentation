# About Data Set

Our dataset contains sales data from an e-commerce site for 2021.
Our dataset contains a total of 6 columns.

customer_id &#8594; Identity information unique to each customer making a purchase

item_id &#8594; Identity information unique to each product purchased

item_name &#8594; Names of purchased items

unit_price &#8594; Unit prices of the products

item_count &#8594; Number of products purchased

purchase_time &#8594; When the customer makes the purchase


In the dataset was defined as the parameters customer_id and unit_price float,
                                             item_id and item_count parameters integer,
                                             item_name and purchase_time parameters object.

Since we don't need to do any mathematical operations with the customer_id and item_id parameters here, they are used as an object; Since we also need the "purchase_time" parameter as a date, we changed it to "datetime". 

Also, because the customer_id parameter comes as an integer, we removed the trailing ".0" values.

Our data set has a total of 16,105,820 rows, 3,706,002 unique item_id and 2,847,919 unique customer_id.

# Brief Description About Segments

**Champions**: Recently Purchased, Often Purchased, and Most Spent. Reward those customers. You can become an early adopter of new products and help promote your brand.

**Loyal Customers**: Shop regularly. Responds to promotions.

**Potential Loyalist**: Recent customers with average frequency. Offer membership or loyalty programs or recommend related products to resell and help them become your loyalists or champions.

**New Customers**: Purchased recently, but not often. Start building relationships with these customers by offering onboarding support and special offers to increase their visits.

**Promising**: New buyers but not much spent.

**Need Attention**: Above-average topicality, frequency and monetary values. I may have bought it recently though.

**About to Sleep**: below-average timeliness and frequency. Lose them if they don't reactivate.

**At Risk**: Some time since purchase. I have to bring her back! Send them personalized reactivation campaigns to reconnect and offer renewals and helpful products to encourage another purchase.

**Can't Lose**: Often bought in the past, but haven't returned it for a long time. Bring them back with relevant promotions and conduct surveys to find out what went wrong and avoid losing them to a competitor.

**Hibernating**: Last purchase was a long time ago and low number of orders. Can be lost.
