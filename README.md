## About the Project 

This project provides a comprehensive analysis of Walmart product data, combining information from two distinct datasets: Walmart E-commerce product listings and Walmart Grocery product data. The goal is to clean, integrate, and analyze this data to uncover insights into product pricing, categories, and other relevant attributes. Data is analyzed to find the most popular brand(s), departments and average prices in different departments as well. 

I've also created a couple Dashboards that can be accessed by the following links:
[Dashboard 1](https://public.tableau.com/app/profile/angel.thompson1715/viz/PriceProject/Dashboard1#1)
[Dashboard 2](https://public.tableau.com/app/profile/angel.thompson1715/viz/PriceProject/Dashboard2#1)


## Data Sources
Two data sources were used from Kaggle website. Both are in CSV format. These must be downloaded in order to run the project. 
- [df - walmart.csv](https://www.kaggle.com/datasets/hikageshinomori/walmart-e-commerce-product-data)
- [df1 - WMT_Grocery_202209.csv](https://www.kaggle.com/datasets/thedevastator/product-prices-and-sizes-from-walmart-grocery)

## Tools Used
    • Pandas: This is a powerful open-source data analysis and manipulation library for Python. Its primary role in this project is:
        ◦ Data Loading: Reading the CSV files (walmart.csv and WMT_Grocery_202209.csv) into DataFrame objects.
        ◦ Data Cleaning: Converting data types and renaming columns.
        ◦ Data Manipulation: Selecting relevant columns and performing operations to create new features.
        ◦ Data Inspection: Providing methods to view data (e.g., head(), dtypes, isnull().sum()).
    • SQL: is utilized to extract raw data from databases. This involves writing queries to select, filter, and join tables to obtain the necessary dataset for analysis and visualizations.
    • Seaborn: This was used to create aesthetically pleasing and informative statistical graphics for exploratory data analysis (EDA). 

## Data Summary

I aimed to find the most popular brands and products and look at the difference in pricing of products as well. I decided to remove unwanted columns at the beginning and instead of filling in null values, I decided to leave them as is to not skew the values with averages that could have thrown the data way off since there were multiple prices in different categories, etc. 

What came as no surprise was that Great Value was the most popular brand, accounting for over 50% of the products. Even though the Pantry department was found to be the one with the most amount of products, Alcohol was the department with the highest total value. Pantry did come in second though. 

I created a couple Tableau Dashboards where you can see visualizations showing average price per department, average price per brand, total spent on top products per department, top 10 brands per category, and top 10 most popular brands. In my Jupyter notebook, I have visualizations showing total products per department, top 10 most popular brands, top 10 brands by average price, price distribution by department, top 10 most expensive products, total value by department, and top 5 subcategories by average price. I did notice with the top 10 most expensive products that there is a Hi Chew candy showing as the 2nd most expensive product, so that price must be entered incorrectly. 

### Running the Program:
This project was created with Python3.13.2

The following is a guide to running the project files locally:

Also, as a reminder, the data sources listed above need to be downloaded as well. 

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


## Project Summary

I used two Walmart data sets for my data analysis as reported above. I looked into finding the most popular brands, products and price variances. I found ‘Great Value’ brand to be the most popular, accounting for over 50% of the products in the data. The average price for ‘Great Value’ branded products was $3.89. The ‘Pantry’ department was the most popular department based on quantity of products. However, the ‘Alcohol’ department was found to have the highest total value. 

I used Python in a Jupyter notebook with pandas and SQL to clean and analyze the data. I was able to merge my two data sets and then create SQL tables to make different visualizations. I also used Tableau to create a couple visualization dashboards as listed below. 

Here are links to my Tableau Dashboards where I created several visualizations. There is one showing the average price per department where we can see that the department ‘Industrial & Scientific’ has the highest average price of $51.84. I also have visualizations showing the total spent on top products per department where the amount of products shown per department is changeable, the average price per brand, the top 10 brands per category, and the top 10 most popular brands. 

[Dashboard 1](https://public.tableau.com/app/profile/angel.thompson1715/viz/PriceProject/Dashboard1#1)
[Dashboard 2](https://public.tableau.com/app/profile/angel.thompson1715/viz/PriceProject/Dashboard2#1)

One limitation I found within the data was that with the top 10 most expensive products that there is a Hi Chew candy showing as the 2nd most expensive product, so I concluded that price must be entered incorrectly. I did decide to leave the data in to show that sometimes data could be entered incorrectly and we might not realize it unless we know what to expect for certain data. I only realized it because I know that candy shouldn’t be as expensive as it is listed in the data. 

In conclusion, we can see how data can be manipulated and used to show the data in an easy to read visual graph. It is important to analyze the data to see if there is data that needs to be removed to not skew the results too much unless we are wanting to see the outliers for analytical purposes. It is also crucial to know the data you are dealing with in order to point out something that is throwing off the data and being reported incorrectly, such as in my example of the Hi Chew candy. 