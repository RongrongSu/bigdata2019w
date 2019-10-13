# bigdata2019w
You can find instructions and details of assignments from https://roegiest.com/bigdata-2019w/syllabus.html.

A0 tasks: 

         (1) Find the 50 most frequently appearing tokens and their frequency in the text of Shakespeare's plays.

         (2) Find a list of words that appear after the word "perfect", on the same line in the text of Shakespeare's plays. 

  
A1 task: 

         (1) Calculate and analyze the pointwise mutual information (PMI) of tokens in the text of Shakespeare's plays
  
* A0 and A1 are done with Python

A2 tasks:
         
         (1) Implement A0 and A1 task with PySpark.
         
         (2) Write the code for the function PMI that will take a positive integer threshold $T$ as an argument, and then return all token pairs that co-occur at least $T$ times in Shakespeare.txt. For each such pair $(x,y)$, the function should also report PMI$(x,y)$, the co-occurrence count of the pair, the number of times $x$ appears, and the number of times $y$ appears.
         
         (3) Write Spark code for the function PMI_one_token, that will take a positive integer threshold $T$ and a sample size $N$ as arguments. For every token $x$ in Shakespeare.txt, your code should find all tokens $y$ that co-occur with $x$ at least $T$ times, as well as PMI$(x,y)$ for each such pair, the co-occurrence count of the pair, the number of times $x$ appears, and the number of times $y$ appears.
         
A3 tasks:

         (1) Use Python and Spark to perform some graph analysis, using a graph of the Gnutella server network.
         
         (2) Write a Spark program to perform personalized page rank over the Gnutella graph for a specified number of iterations, and of course a specific node.
         
         (3)Modify your personalized page rank implementation from Question 2 so that it iterates until the maximum node change is less than $\frac{0.5}{N}$, where $N$ represents the number of nodes in the graph.
         
A4 tasks:

         (1) Using Python and Spark to perform some simple analyses on relational (tabular) data. (Hive)
         
         (2) Implement the function five_highest_totalprice_orders_sql() that will return the ORDERKEY, ORDERDATE, and TOTALPRICE of the five orders with the highest TOTALPRICE.
         
         (3) Implement the function five_highest_totalprice_orders_dtf() to answer the same query you answered in Question 1, but this time do not use the sql method.
         
         (4) Implement the function cust_most_recent_order_sql(custkey) that takes a Customer Key as an input and returns the customer's name as well as the ORDERDATE and TOTALPRICE of that customer's most recent order.
         
         (5) Answer the same query you answered in Question 3, but this time do not use the sql method.
          
         (6) Implement distinct_supplied_parts(nname) that will return the number of distinct parts supplied by suppliers that are located in the given nation.
         
         (7) Implement count_suppliers_brand_per_nation(bname) that takes a brand name as input, outputs should be a table of nations and their supplier counts.
         
         (8) Write code for the function order_number_per_customer_nation(nname) that will return, for a given nation name, for each year, the total number of orders placed by customers from the specified Nation, ordered by descending number of orders.
         
A5 tasks:

         (1) Use Python and Spark to perform spam detection. 
         
         (2) Build spam prediction models, using training data sets and stochastic gradient descent (SGD).
         
         (3) Use these models to predict whether the documents in a test data set are spam.
