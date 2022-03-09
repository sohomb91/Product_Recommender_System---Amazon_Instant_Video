## Amazon Instant Video -- Product Recommender System

Here, we will be attemting to build an intermediate Product Recommendation Engine for Amazon Instant Video products targeted for sellers looking to sell the AIV products based on user ratings and past sales.

We will be looking to build the same based on the combined factor of the product ratings, given on the AIV products by the users, with the past sales figures of the products (giving a weightage of 60% & 40% to the respective features). 


## Data

These dataset is a subset of the original [Amazon Product Data](https://jmcauley.ucsd.edu/data/amazon/) dataset, which includes no metadata or reviews, but only (User, Asin, Rating, Timestamp) tuples.\
This dataset also does not include the `sales` feature, which we will utilize here in modelling; rather, we will generate the same figures randomly for each Asin(item_id).

For more information on the dataset or for the complete `Amazon Product Data` dataset or similar, please visit: https://jmcauley.ucsd.edu/data/amazon/

**Data Dictionary:**
 - ***User:*** Unique user id who have rated a particular Asin/Product/Item.
 - ***Asin:*** Unique item id or product id which have been rated by a particular user.
 - ***Rating:*** Unique rating given to that product (1: Lowest and 5: Highest).
 - ***Timestamp:*** Unix epoch timestamp of when a particular user has rated that product.
