# Instacart-Market-Basket-Analysis
Model based on instacart Market basket analysis using Tenserflow Framework

# Goal of Model
The goal is to predict which products will be in a user's next order. The dataset is anonymized and contains a sample of over 3 million grocery orders from more than 200,000 Instacart users. For each user, we provide between 4 and 100 of their orders, with the sequence of products purchased in each order. We also provide the week and hour of day the order was placed, and a relative measure of time between orders.

# File descriptions
Each entity (customer, product, order, aisle, etc.) has an associated unique id. Most of the files and variable names should be self-explanatory.

# aisles.csv
 `aisle_id,aisle
 
 1,prepared soups salads  
 2,specialty cheeses  
 3,energy granola bars 
 ...`

# departments.csv
`department_id,department\

 1,frozen  
 2,other  
 3,bakery 
 ...`

# order_products__*.csv
These files specify which products were purchased in each order. order_products__prior.csv contains previous order contents for all customers. 'reordered' indicates that the customer has a previous order that contains the product. Note that some orders will have no reordered items. You may predict an explicit 'None' value for orders with no reordered items

# orders.csv
This file tells to which set (prior, train, test) an order belongs. You are predicting reordered items only for the test set orders. 'order_dow' is the day of week.

