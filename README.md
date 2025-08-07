## About the Project

This project provides a comprehensive analysis of Walmart product data, combining information from two distinct datasets: Walmart E-commerce product listings and Walmart Grocery product data. The goal is to clean, integrate, and analyze this data to uncover insights into product pricing, categories, and other relevant attributes. Data is analyzed to find the most popular brand(s), departments and average prices in different departments as well. 

I've also created a couple Dashboards that can be accessed by the following links:
https://public.tableau.com/app/profile/angel.thompson1715/viz/PriceProject/Dashboard1#1
https://public.tableau.com/app/profile/angel.thompson1715/viz/PriceProject/Dashboard2#1


## Data Sources
Two data sources were used from Kaggle website. Both are in CSV format. 
- [walmart.csv](https://www.kaggle.com/datasets/hikageshinomori/walmart-e-commerce-product-data)
- [WMT_Grocery_202209.csv](https://www.kaggle.com/datasets/thedevastator/product-prices-and-sizes-from-walmart-grocery)


### Running the Program:
This project was created with Python3.13.2

The following is a guide to running the project files locally:

1. Fork the repository [repo link](https://github.com/angeldthompson/price_project.git)  
2. Clone the repository to your Github account
3. Access the repository from your command line or preferred CMD software
4. Install a virtual environment. The command in Gitbash is *python -m venv venv*
5. Activate the virtual environment. The command in Gitbash is *source venv/scripts/activate*
6. Install the *requirements.txt* file to install necessary packages by running *pip install requirements.txt* 

## Data Dictionary 
This provides a comprehensive data dictionary for variables used in the merged and cleaned data from  both walmart.csv and  WMT_Grocery_202209.csv data sets

- Product_NAME - The full name of the product.
- URL - The URL link to the product page on Walmart's website.
- BRAND - The brand name of the product.
- SKU - The Stock Keeping Unit, a unique identifier for the product.
- DEPARTMENT - The main department in which the product is categorized.
- PRICE - The current selling price of the product.
- CATEGORY - The first sub-category of the product.
- SUBCATEGORY - The second sub-category of the product.
- PRODUCT_SIZE - The size or quantity of the product (e.g., "12 oz", "Large").
- SCRAPED_AT - The date and time when the product data was collected.
- PRICE_TIER - New column created to sort products into low, medium, and high price tiers


## Data Summary
I decided to remove unwanted columns at the beginning and instead of filling in null values, I decided to leave them as is to not skew the values with averages that could have thrown the data way off since there were multiple prices in different categories, etc. 

What came as no surprise was that Great Value was the most popular brand, accounting for over 50% of the products. Even though the Pantry department was found to be the one with the most amount of products, Alcohol was the department with the highest total value. Pantry did come in second though. 