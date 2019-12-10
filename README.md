KaggleCompetition_Instacart_Market_Basket_Analysis

1. Introduction

In this competition, Instacart is challenging the Kaggle community to use anonymized data on customer orders (3 Million Instacart Orders, Open Sourced.) over time to predict which previously purchased products will be in a user’s next order. 

Data description: https://tech.instacart.com/3-million-instacart-orders-open-sourced-d40d29ead6f2

Data link: https://www.instacart.com/datasets/grocery-shopping-2017 

Kaggle competition link: https://www.kaggle.com/c/instacart-market-basket-analysis/overview

There are 6.csv files which provide data on aisles, departments, products, and order information.

    aisles.csv: Information regarding the aisle an item can be found (prepared soups/salad, speciality cheeses, etc.)
    
    departments.csv: Information regarding the department an item can be found (frozen, bakery, etc.)
    
    product.csv: Information regarding the product (product ID, which department/aisle it can be found), ~50,000 products.
    
    order_products_prior.csv: Data regarding orders that users previously purchased
    
    order_products_train.csv: Data regarding the last order for a user
    
    orders.csv: Information on the order each user put in, including the day of week, hour of day, and the number of days since previous order

Based on these files, we are able to perform feature engineering, and build train and test datasets.

2. Feature Engineering
Feature engineering is the process of extracting relevant information from the existing data and constructing new features. 

In this project, 41 features were created from the following four dimensions: User- and Product-based features, User-Based features, Product-Based features and Datetime-Based features.

    1) User- and product-based features describes a specific user’s interactions with a specific product. 
       One example is: The number of orders from this user that includes this product.
    
    2) User-Based features describes the purchasing pattern for a specific user.
    
    3) Product-Based features describes purchasing pattern for a specific produc across all users.
    
    4) Datetime-Based features describes the purchasing pattern for users within a timeframe.
    
3. Machine Learning Model

XGBoost was used to perform predictions.
    
    






