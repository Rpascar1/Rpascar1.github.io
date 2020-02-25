---
layout: post
title:      "Simple SQL Dataset "
date:       2020-02-25 13:59:15 -0500
permalink:  simple_sql_dataset
---


Before graduation I had thought about what I would do after graduation in terms of continued learning. For me, SQL seemed like the obvious choice. 
While in the FlatIron program, basic SQL was taught. After this however Rails relied on Active Record to abstract away writing much of SQL call code. 
I spoke with numerous senior developers of varying backgrounds and my feelings about the importance of SQL were more than confirmed.

     
```
SELECT customerName,
	COUNT(*) AS 'number of orders'
    FROM customers
    	INNER JOIN orders
    	ON orders.customerID = customers.customerID
GROUP BY customers.customerID;  

```

I began to work on a data det running calls just to see what would happen using one of Steven Grider’s beginner test data set lessons.  This dataset can be found here:

[SQL Dataset](https://www.w3schools.com/sql/trysql.asp?filename=trysql_op_or)

I quickly figured out that I remembered a lot more than I originally had thought. After all the other code I have written in the last 9 months, the base SQL calls felt extremely intuitive. I began to string more and more together in almost plain English.
 
![imgur](https://imgur.com/GE3Z8wU.gif)

