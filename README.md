# Yelp Review Analysis

Yelp is currently the most widely used restaurant and merchant information software across United States. However, Yelp only provides us a holistic view about restaurant, such as giving overall review score or ratings and only a few reviews out of thousands of reviews.  

The objective of this project is to help yelp users, whether they are business owners or consumers, to find information that better meet their preferences. Specifically, our group mainly focused on improving customers’ understanding of restaurants, new business owners'market knowledge, and existing merchants’ awareness about restaurants’ features.   

* We first obtained and extracted data from Yelp open source, United States Census Bureau, and a research group from Stony Brook University. The data consists Yelp businesses, users, reviews, U.S.income, and fake review labeled data. 

* After cleaned the data, we created a SQL database to store Yelp review data. Our database consists of Yelp businesses, users, reviews_fact_table, and income tables that describe different aspects of the data, which allow us to do effective joining and querying.

* In the first part of this project, we examined the fake review detection data, which consists of 350,000 user reviews. The true and fake reviews in the dataset help us trained a model that predicts the validity of a given review (fake/true).

* In the second part of this work, we examined Yelp’s merchant review data with machine learning techniques as well as natural language processing tools to provide consumers and existing merchants insights from the data. Fitting statistical models to the data, we are able to access the most relevant keywords in the reviews that affect review scores.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine.

 * *In order to obtain the raw data:*
    1. You would need to download Yelp Open Dataset from https://www.yelp.com/dataset. We mainly focus on business.json, review.json, and        users.json in our project. 
    2. You would need to download Fake review labeled data by following the link in **Machine Learning Training Set.txt** file.
    3. You would be able to directly download **income.csv** and **zip_code_states.csv** from the **data** folder.
 
 
 * *In order to obtain the cleaned data:*
    1. You would be able to obtain a cleaned and merged income and zipcode csv by running **Clean_income_zipcode_data.py** in the **script** folder,or you can just download the **income_zipcode.csv** from **data** folder
    2. You would be able to obtain a cleaned business.csv by just downloading the **business_data.csv** in **data** folder.
    3. You would be able to obtain a cleaned review.csv and users.csv by running **Load&Clean Yelp Dataset.ipynb** in the **script** folder. 
 
 
 * *In order to build the SQL database and have a preliminary view about the data:*
    1. You would need to run **SQL Database & Preliminary Data Visualization.ipynb** in the **script** folder. You would also need to obtain cleaned reviews, income_zipcode, users, and business data and put them in a data folder from the previous section. These data will be used to populate our SQL database. 
 
 
 * *In order to visualize some of the data:*
    1. You would need to run **Visualization_for_Review_Business.ipynb** in the **script** folder.
 
 
 * *In order to run fake review detection machine learning model and using filtered true reviews to extract keywords:*
    1. You would first need to have fake review labeled data obtained from previous section. Then you would need to run **Machine Learning.ipynb** in the **script** folder to predict whether our current reviews are deceptive or trustworthy.
    2. After running **Machine Learning.ipynb**, you would need to run **word_cloud & feature extraction.ipynb** to find the key insights about each restaurant.
 
 
